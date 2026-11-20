# Image-to-Video Prototype — FrameFlow Studio

Google Flow (Veo 3.1) se inspired working prototype. Image upload karo, motion prompt do, duration chuno, aur 1080p HD video generate karo.

## Features

- Image upload (drag & drop) + 3 sample images
- Motion prompt with cinematic enhancer
- Duration: **10 / 15 / 20 / 25 / 30 seconds**
- 6 camera motions: Zoom, Pan, Orbit, aur bhi
- Motion intensity aur ratios: 16:9 / 9:16 / 1:1
- Output: **1920 x 1080 (1080p HD)**, real-time canvas recording
- Stage-by-stage progress, animated preview, clips history, downloadable video

## Flow ki asal limit (important)

Google Flow / Veo 3.1 mein ek clip max **8 second** ki banti hai. Is liye 10-30 second ki video kayi clips ko jor kar (Scene Builder / Extend) banti hai. Ye prototype usi flow ko samjhata hai aur demo video browser mein banata hai.

Prototype mein download **WebM** file milti hai; production version mein ye **MP4** hogi.

## Run / Test

Koi build step nahi hai. Sirf static file hai.

```bash
# Option 1 — seedha browser mein kholein
# index.html par double-click karein

# Option 2 — local server (recommended)
python3 -m http.server 8000
# phir browser mein kholein: http://localhost:8000
```

Phir:
1. Image upload karein ya sample chunein
2. Duration chunein (10, 15, 20, 25 ya 30 sec)
3. Generate dabayein, preview dekhein, video download karein

## Files

- `index.html` — poora prototype (self-contained)
- `README.md` — ye file
