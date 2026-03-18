# Videos Folder

Place your video files here. The site supports `.mp4` format.

**Example structure:**
```
static/videos/
├── my-first-video.mp4
├── my-second-video.mp4
└── phonk-edit.mp4
```

Then reference them in the video content files with the `videoFile` front matter:

```yaml
---
title: "My Cool Video"
description: "A brief description"
videoFile: "my-first-video.mp4"
---
```

The video files should be placed directly in this `videos/` folder, and the `videoFile` parameter should just be the filename.
