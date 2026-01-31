# Audio Noise Removal Using MATLAB

This project demonstrates **noise removal from an audio file** using MATLAB. A **voice recording** contaminated with a sine wave interference (e.g., beep at 240 Hz) is processed using **IIR notch and peak filters** to recover the original signals.

---

## Features

- Mixes **voice and interference signals** into a single audio file.
- Performs **time-domain and frequency-domain analysis**.
- Implements **IIR Notch Filter** to remove target frequency noise (voice recovery).
- Implements **IIR Peak Filter** to isolate interference (sine wave recovery).
- Computes **validation metrics**:
  - Pearson correlation between original and recovered signals
  - Signal-to-Noise Ratio (SNR)
- Saves cleaned audio files (`recovered_voice.wav`, `recovered_sine.wav`).
- Supports **resampling** and **stereo-to-mono conversion** automatically.

---

## Usage

1. Place your audio files in the project folder:
   - `voice.mp3` (voice signal)
   - `240sinwave.wav` (interference)
2. Open `AudioNoiseRemoval.m` in MATLAB.
3. Run the script:
   - Mixed audio will be saved as `mixed_audio.wav`.
   - Recovered signals will be saved as `recovered_voice.wav` and `recovered_sine.wav`.
   - Plots of **time-domain and frequency-domain signals** will be displayed.
   - Validation metrics (correlation, SNR) are printed in MATLAB console.
4. Optional: Playback of audio occurs automatically during the script.

---

## Workflow

1. **Load Audio Files** – Resample and convert to mono if necessary.
2. **Mix Signals** – Combine voice and sine wave.
3. **Frequency Analysis** – Compute FFT and visualize spectra.
4. **Filter Design** – Create notch filter for noise removal and peak filter for interference isolation.
5. **Apply Filters** – Recover original signals.
6. **Validation** – Evaluate correlation and SNR.
7. **Audio Playback** – Listen to mixed and cleaned signals.

---

## Skills Demonstrated

- MATLAB Programming
- Digital Signal Processing (DSP)
- Audio Signal Analysis
- Filter Design (Notch and Peak IIR)
- Frequency-Domain Analysis and FFT
- Signal Validation Metrics (SNR, Correlation)

---

## Author

**Mushaf Iftikhar**  
Email: mushafiftikharawan@gmail.com

---

## License

This project is open-source and free to use for educational purposes.

---

