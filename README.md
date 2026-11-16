# ATC Voice Trainer

A browser-based aviation radiotelephony practice tool. It plays ATC instructions, captures a pilot readback, displays speech-recognition output, and provides a simple practice score.

## Open the app

After GitHub Pages is enabled, the site will be available at:

https://beakwings123-sketch.github.io/atc-voice-trainer/

## Current features

- Built-in ATC practice scenarios: IFR clearance, taxi, climb/frequency change, weather deviation and go-around.
- Controller instruction playback using the browser's speech synthesis.
- Pilot response recognition using the browser Web Speech API.
- Microphone audio recording and playback (where supported).
- Basic keyword and number matching feedback.
- Import custom practice scripts as TXT or DOCX.
- Responsive layout for desktop and mobile browsers.

## Import format

Use a blank line between exchanges. Each exchange should contain an `ATC:` line and optionally a `PILOT:` example:

```text
ATC: Shandong Airlines 218, climb to flight level 280. Contact Shanghai Control on 125 decimal 75.
PILOT: Climb to flight level 280, contact Shanghai Control 125 decimal 75, Shandong Airlines 218.

ATC: Shandong Airlines 218, go around. Fly runway heading and climb to 3,000 feet.
PILOT: Going around, runway heading, climb to 3,000 feet, Shandong Airlines 218.
```

## Browser and privacy notes

- Recommended: a recent version of Google Chrome or Microsoft Edge.
- Microphone access requires HTTPS (GitHub Pages provides HTTPS) and user permission.
- Speech synthesis voices depend on the browser and operating system.
- Web Speech API recognition availability varies by browser and may send audio to a browser vendor's recognition service; it may require an internet connection.
- Imported documents and audio recordings are handled in the browser by this static app. DOCX import loads Mammoth.js from a CDN.
- No training document is intentionally uploaded to this repository by the app.

## Important

This is an independent practice aid. Its score is a simple keyword/number comparison and is **not** an official ICAO, PEPEC, EPTA, airline or regulator assessment. Always follow approved company procedures and current phraseology standards.

## Enable GitHub Pages

In the repository, open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select branch **main** and folder **/(root)**, then save. Wait for GitHub Pages to finish publishing.
