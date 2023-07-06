# Useful FFMPEG

## Resize to fit with Aspect Fit

```bash
export NEW_WIDTH=1080
export NEW_HEIGHT=1920
ffmpeg -i THRESHOLD-converted.mp4 -vf "scale=-1:$NEW_HEIGHT:force_original_aspect_ratio=increase,crop=$NEW_WIDTH:$NEW_HEIGHT,pad=$NEW_WIDTH:$NEW_HEIGHT:(ow-iw)/2:(oh-ih)/2:black" output1.mp4
```
