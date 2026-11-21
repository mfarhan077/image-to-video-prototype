# AutoFlow AI Studio

Premium AI video creation platform — static single-file build.

## Run locally

```bash
git clone https://github.com/mfarhan077/image-to-video-prototype.git
cd image-to-video-prototype
python3 -m http.server 8000
```

Open http://localhost:8000

## What is inside

- Dashboard, Projects, AI Video Generator, Storyboard Studio
- Automotive Studio — "RAV4 Launch Film" project with a 20-scene plan for the 2026 Toyota RAV4 in Pearl White, preloaded
- Image Generator, Voiceover Studio, Video Editor, YouTube Studio, Asset Library, Templates, Settings
- Projects are saved in the browser (localStorage)

## Providers

Cloud video providers (Veo / Runway) and ElevenLabs voice are NOT connected yet.
Settings shows what API key is needed. Render requests are recorded as
"Needs provider" — no fake generation.
