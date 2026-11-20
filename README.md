# Image-to-Video Prototype — FrameFlow Studio

Google Flow (Veo 3.1) se inspired working prototype. Image upload karo, motion prompt do, duration aur ratio chuno, aur HD video generate karo.

## Features

- Image upload (drag & drop, bada choose box, thumbnail + size/resolution preview, Change button) + 3 sample images
- Motion prompt with cinematic enhancer
- Duration: **10 / 15 / 20 / 25 / 30 seconds**
- 6 camera motions: Zoom, Pan, Orbit, aur bhi
- Motion intensity
- Ratios (7): **16:9 (1920x1080, YouTube), 9:16 (1080x1920, Reels / TikTok / Shorts), 1:1 (1080x1080), 4:5 (1080x1350), 3:4 (1080x1440), 4:3 (1440x1080), 21:9 (2520x1080, cinematic)**
- Output: ratio ke exact size mein, real-time canvas recording
- Stage-by-stage progress, animated preview, clips history, downloadable video (file name mein ratio bhi likha hota hai)

## Target style

Presenter / talking-head video jaisi — jaise 9:16 vertical video mein ek presenter mic ke saamne bol rahi ho. Prototype mein image ko presenter-style halki movement (zoom / sway) ke sath animate kiya jata hai.

## Flow ki asal limit (important)

Google Flow / Veo 3.1 mein ek clip max **8 second** ki banti hai. Is liye 10-30 second ki video kayi clips ko jor kar (Scene Builder / Extend) banti hai. Ye prototype usi flow ko samjhata hai aur demo video browser mein banata hai.

Prototype mein download **WebM** file milti hai; production version mein ye **MP4** hogi. Asal AI lip-sync (honth hila kar bolna) browser prototype mein nahi hota — wo Veo / AI talking-head API se hota hai production mein.

## Run / Test

Koi build step nahi hai. Sirf static file hai.

```bash
# Repo ko update karein (pehli dafa clone karein)
git clone https://github.com/mfarhan077/image-to-video-prototype.git
cd image-to-video-prototype
git pull

# Local server (recommended)
python3 -m http.server 8000
# phir browser mein kholein: http://localhost:8000
```

Phir:
1. Image upload karein ya sample chunein
2. Ratio chunein — 9:16 test ke liye Reels / Shorts style
3. Duration chunein (10, 15, 20, 25 ya 30 sec)
4. Generate dabayein, preview dekhein, video download karein

## Files

- `index.html` — poora prototype (self-contained)
- `README.md` — ye file
