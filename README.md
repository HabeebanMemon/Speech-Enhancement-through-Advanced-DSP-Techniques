# Speech-Enhancement-through-Advanced-DSP-Techniques


A sophisticated Python implementation of real-time speech recovery using Digital Signal Processing (DSP) to isolate voice from background noise.

##  Project Overview
Background noise often compromises the quality of communication in telecommunications and hearing aids. This project addresses the challenge by implementing a frequency-domain enhancement system that significantly boosts the clarity and intelligibility of speech signals.



##  Key Features
* **Spectral Subtraction:** Attenuates noise by subtracting estimated noise power from the total signal spectrum.
* **STFT & ISTFT:** Utilizes Short-Time Fourier Transform for localized frequency analysis and Inverse STFT for high-fidelity audio reconstruction.
* **Butterworth Band-Pass Filtering:** Specifically tuned to the human vocal range (approx. 300Hz - 3400Hz) to eliminate out-of-band interference.
* **Noise Gating:** Intelligent thresholding to silence non-speech segments.
* **Quantitative Analysis:** Automated calculation of Signal-to-Noise Ratio (SNR) improvements.



##  Technical Workflow
1. **Windowing:** Applying Hamming windows to minimize spectral leakage.
2. **FFT Analysis:** Converting audio frames into the frequency domain.
3. **Noise Estimation:** Sampling initial silent frames to build a noise profile.
4. **Magnitude Subtraction:** Subtracting the noise floor while preserving phase information.
5. **Signal Synthesis:** Overlap-add method for seamless time-domain reconstruction.

##  Evaluation Results
The system provides a comprehensive evaluation suite:
* **Waveform Comparison:** Visual proof of amplitude normalization and noise floor reduction.
* **SNR Metrics:** Comparison of `Original SNR` vs. `Enhanced SNR` in decibels (dB).
* **Spectrograms:** Heatmaps showing the effective removal of constant-frequency noise and broadband hiss.

##  Tech Stack
* **Language:** Python 3.10+
* **Libraries:** NumPy (Matrix Math), SciPy (Filter Design), Librosa (Audio Processing), Matplotlib (Data Visualization).

---
**Developed by:** Habeeban Memon
**Academic Supervision:** Engr. Asif Ali (Sukkur IBA University)
