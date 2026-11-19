# HSP Home Analyzer

Local browser-based audio engineering and monitoring lab (Royal Purple & Black edition).

## Features
- **Local-First Audio Analysis:** Decodes WAV, MP3, M4A, FLAC, and AIFF files directly in the browser using Web Audio API—no files are uploaded to any server.
- **Signal Metrics:** Measures Sample Peak (dBFS), RMS (dBFS), Duration, and Crest Factor (dB).
- **Waveform & Multi-Window FFT Spectrum:** Averages power across up to 16 evenly spaced 8,192-sample windows so quiet intros or middle sections do not skew the frequency plot.
- **Frequency-Band Balance & Diagnostics:** Breaks down energy across Sub, Bass, Body, Low Mids, Mids, Presence, Sibilance, and Air with conservative EQ starting suggestions.
- **Transport Controls:** True Play/Pause/Resume with timeline scrubbing (`0:00` timecode readout), mobile-friendly for iOS Safari.
- **Offline Preview Processing & Export:** Applies high-pass, 300 Hz low-mid, and 3 kHz presence filters offline and exports a new processed `.wav` file plus a `.txt` analysis report.

## Deployment (GitHub Pages)
1. Upload `index.html` and `README.md` to the root of your repository (`main` branch).
2. Ensure `index.html` is all lowercase.
3. Open **Settings -> Pages**, select **Deploy from a branch**, choose `main` and `/ (root)`, and click **Save**.
4. Wait 60–90 seconds for the **Actions** workflow (`pages build and deployment`) to turn green, then open your live `github.io` URL.
