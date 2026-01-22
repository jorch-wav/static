# Video Setup Instructions

You need to add two video files to this directory:

1. **video1.mp4** - Static/noise video (the curtain layer)
2. **video2.mp4** - Music video (the content underneath)

## From your Raspberry Pi Static folder:

```bash
# Copy the videos
cp ~/Static/video1_480p.mp4 ~/static-web/video1.mp4
cp ~/Static/video2_480p.mp4 ~/static-web/video2.mp4
```

Or if you prefer higher quality (may affect performance):
```bash
cp ~/Static/video1_720p.mp4 ~/static-web/video1.mp4
cp ~/Static/video2_720p.mp4 ~/static-web/video2.mp4
```

## Alternative: Create test videos

If you want to test without the original videos, you can use any two MP4 files:
- video1.mp4 should be your "static curtain" effect
- video2.mp4 should be your "music video" content

**Note:** For GitHub Pages deployment, keep videos under 100MB total if possible.
For larger videos, consider hosting them elsewhere (YouTube, Vimeo, CDN) and loading via URL.
