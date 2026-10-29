# Subliminal Studio

A website and browser app for making subliminal videos. Add an affirmation
recording, set it under background sound, and export a finished video sized for each platform.

Everything renders on your device. Nothing is uploaded.

## Pages

| File | Page |
| --- | --- |
| `index.html` | Home page |
| `studio.html` | The studio app |
| `guide.html` | How to write, record, mix and post a subliminal |
| `faq.html` | Common questions |
| `privacy.html` | What happens to your files |
| `404.html` | Not-found page for GitHub Pages |
| `assets/` | Shared stylesheet and icon |

## Use it

Open `index.html` in a recent browser (Chrome, Edge or Safari work best), or serve the folder:

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

It's published with GitHub Pages at https://iritikarani.github.io/Subliminal/ by
`.github/workflows/pages.yml`, which redeploys on every push. Pages must be set to deploy from
**GitHub Actions** (Settings → Pages → Build and deployment → Source).

## What it does

1. **Voice**: load an audio or video file, then set the voice level (−45 to 0 dB), the number of
   layers (1–5, spread across left and right), the speed, the pause between repeats, and the length.
2. **Sound**: add generated background sounds (rain, ocean, wind, fireplace, dream pad, pink or
   brown noise, a 6 Hz theta binaural beat), your own music if you want, and fade in/out.
3. **Format**: choose 9:16, 16:9, 1:1 or 4:5, at 1080p or 720p.
4. **Look**: pick a background (sparkles, aurora, night sky, voice orb, waveform, or your own photo),
   a colour palette, a title and subtitle, a font, on-screen affirmations and your handle.
5. **Export**: create an MP4 video (H.264/AAC through WebCodecs where the browser supports it),
   or audio only.

Your settings are kept in the browser's local storage between visits.
