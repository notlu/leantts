# LeanTTS Audio Demo

Audio demonstrations for **LeanTTS: Efficient Full-Stack Bilingual TTS for Zero-Shot Cloning and Voice Customization**.

This repository contains a static, browser-based listening demo for comparing LeanTTS model variants on English and Chinese speech synthesis. No installation or build step is required.

## Demo Contents

### Zero-Shot Voice Cloning

- 8 English samples and 8 Chinese samples from the SeedTTS evaluation set
- A reference recording and transcript for each sample
- Side-by-side outputs from:
  - LeanTTS 25M
  - LeanTTS 13M
  - LeanTTS 13M 4-step

### Custom Voice

- Demonstrations from 8 speakers
- English and Chinese synthesis examples
- A reference recording for each speaker
- LeanTTS 13M 4-step generation results

## View the Demo Locally

Clone the repository and start a local HTTP server:

```bash
git clone https://github.com/notlu/leantts.git
cd leantts
python3 -m http.server 8765
```

Then open [http://localhost:8765](http://localhost:8765) in a browser.

You can also open `index.html` directly, although a local HTTP server is recommended for more consistent audio playback across browsers.

## Repository Structure

```text
.
├── index.html                 # Demo interface
├── 01_teacher25m/             # LeanTTS 25M outputs
├── 02_teacher13m/             # LeanTTS 13M outputs
├── 04_fixed4_update10k16k/    # LeanTTS 13M 4-step outputs
├── 06_custom_voice/           # Custom Voice references and outputs
└── 07_seedtts_references/     # Zero-shot reference recordings
```

All audio is loaded through relative paths, so the demo can be hosted as a static website, including with GitHub Pages.

## Authors

**Yuheng Lu et al.**

1. Tianjin University, Tianjin, China
2. Didichuxing Co. Ltd., Beijing, China

