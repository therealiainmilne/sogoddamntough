# So Goddamn Tough - Setup Guide

Your TikTok-style video feed is ready!

## How to Add Videos

### 1. **Add your video file**
   - Place your MP4 video in `static/videos/`
   - Example: `static/videos/my-video.mp4`

### 2. **Create a video entry**
   - Create a new `.md` file in `content/videos/`
   - Name it something like `my-video.md`
   - Add this front matter:

```yaml
---
title: "Your Video Title"
description: "A short description of the video"
videoFile: "my-video.mp4"
date: 2026-03-17
draft: false
---

Optional longer description or notes about the video.
```

### 3. **Remove sample videos** (optional)
   Delete these when you add your own:
   - `content/videos/sample-1.md`
   - `content/videos/sample-2.md`

## How to Use

- **Scroll Down**: Wheel scroll, arrow keys, or swipe on mobile
- **Scroll Up**: Same controls in reverse
- Progress bar at the bottom shows your position in the feed
- Counter shows current video / total videos

## Building & Deploying

### Local testing:
```bash
hugo server
```
Then visit `http://localhost:1313`

### Deploy to Netlify:
1. Push your repo to GitHub
2. Connect to Netlify (free hosting)
3. Build command: `hugo`
4. Publish directory: `public`

## Video Tips
- **Format**: MP4 is recommended (best browser support)
- **Size**: Try to keep videos under 20MB each for faster loading
- **Duration**: Works best with videos 15-60 seconds long
- **Aspect ratio**: Vertical (9:16) looks best on mobile

## Customization

All styling is in `layouts/index.html` under the `<style>` tag. You can:
- Change colors (gradients, text colors)
- Adjust video sizing
- Modify animations
- Change the scroll cooldown (currently 800ms)

Good luck! 🚀
