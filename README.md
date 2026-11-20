# Image-to-Video Prototype — FrameFlow Studio

Google Flow se inspired, Flow jaisa professional studio. Image upload karo, prompt aur bolne wali script likho, duration aur ratio chuno, aur HD video generate karo.

## Flow jaisa format (v4)

- Modes: Text to Video, Frames to Video, Ingredients to Video, Presenter mode
- Model: Veo (Flow style), Outputs, Scene Builder, Extend, camera controls
- Image upload: drag & drop tray, click se select, preview mein poori image (contain, kabhi crop nahi)
- Prompt + speaking script: lambi prompt / script likh sakte hain, koi 300 character limit nahi. Character script ke mutabiq bole ga.
- Voice options: 4 awazein, preview mein bolte hue subtitles
- Duration: **10 / 15 / 20 / 25 / 30 seconds**
- Ratios (7): **16:9 (1920x1080, YouTube), 9:16 (1080x1920, Reels / TikTok / Shorts), 1:1 (1080x1080), 4:5 (1080x1350), 3:4 (1080x1440), 4:3 (1440x1080), 21:9 (2520x1080, cinematic)**
- Library (Meri Videos): har bani hui video record hoti hai — prompt, script, duration, ratio aur Ready status ke sath, Play / Download / Phir Banao / Delete

## Target style

Presenter / talking-head video — jaise 9:16 vertical video mein ek presenter mic ke saamne bol rahi ho. Forest prompt example: black background, forest, natural head movement aur hand gestures, warm golden light, slow push-in, photorealistic, 24fps.

## Flow ki asal limit (important)

Google Flow / Veo 3.1 mein ek clip max **8 second** ki banti hai. Is liye 10-30 second ki video kayi clips ko jor kar (Scene Builder / Extend) banti hai. Ye prototype usi flow ko samjhata hai aur demo video browser mein banata hai.

Prototype mein download **WebM** file milti hai; production version mein ye **MP4** hogi. Asal AI lip-sync / voice production mein Veo / AI talking-head API se aata hai — prototype mein ye preview simulation hai.

## Run / Test

Koi build step nahi hai. Sirf static file hai.

```bash
git clone https://github.com/mfarhan077/image-to-video-prototype.git
cd image-to-video-prototype
git pull

# Local server (recommended)
python3 -m http.server 8000
# phir browser mein kholein: http://localhost:8000
```

Phir:
1. Image upload karein ya sample chunein
2. Prompt aur script likhein
3. Ratio chunein — 9:16 test ke liye Reels / Shorts style
4. Duration chunein (10, 15, 20, 25 ya 30 sec)
5. Generate dabayein, preview dekhein, video download karein

## Files

- `index.html` — poora prototype (self-contained)
- `README.md` — ye file
