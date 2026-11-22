# RO’Lyfe DJ Studio

A responsive, browser-based dual-deck DJ workspace with four selectable controller layouts.

**Live site:** https://rolrichman.github.io/rolyfe-dj-studio/

## Controller layouts

- **Classic Dual Deck** — familiar side-by-side decks and mixer.
- **Club Pro** — expanded deck controls and a larger performance workspace.
- **Battle / Scratch** — prominent jog wheels and cue pads.
- **Minimal Performance** — compact touch-first controls for smaller screens.

All layouts use the same two-deck audio engine and preserve the current session while switching.

## Current capabilities

- Local audio file loading (no upload); dual independent playback.
- Browser Web Audio mixing graph, master gain, channel levels and equal-power crossfader.
- Three-band EQ, filter, channel gain and pitch/tempo control.
- Waveform drawing from decoded audio, tap/click waveform seeking and live playhead position.
- Live per-deck signal meters driven by Web Audio analyser nodes.
- Local BPM estimate from an onset-envelope autocorrelation pass.
- Approximate musical-key estimate from FFT chroma energy.
- Tempo sync helper (tempo ratio only; not beat-grid phase alignment).
- Jog-wheel seek/scratch gesture, cue-to-start, four hot-cue slots and a four-beat loop.
- Responsive layouts and a collapsible RO’Lyfe Co-Pilot that describes the actual local analysis state.

## Important limits

This is a browser prototype, not a replacement for licensed professional DJ software. BPM and key are estimates and can be wrong on sparse, syncopated, noisy, or harmonic material. Beat display is a simple elapsed-time estimate; the app does not yet derive a reliable beat grid or phrase map. Tempo sync changes Deck B playback rate but does not phase-lock beats. Hot cues and loops are session-only and are not persisted. Scratch is a basic jog seek gesture, not timecode vinyl emulation. The Co-Pilot is currently local rule-based guidance, not a connected generative AI service.

For best results use a current Chrome-based browser and common audio formats such as MP3, WAV, AAC or M4A. Audio playback requires a user gesture. Performance and supported formats vary by device/browser.

## Use

1. Open the live site.
2. Tap **Enable Audio**.
3. Load an audio file into Deck A and/or Deck B.
4. Use Play, Cue, pitch, EQ, filter, hot cues, loops and jog wheels.
5. Move the crossfader to blend decks.
6. Switch layouts at any time.

## Privacy

Selected audio is decoded and processed locally in the browser. This app does not upload selected audio files.
