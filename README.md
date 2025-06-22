# 🎧 AudioFusionX – Vocal & BGM Mixer with DSP Analysis

Welcome to **AudioFusionX**, a Python-based audio signal processing project developed during our lab sessions. This tool loads separate **vocal** and **background music (BGM)** audio files, mixes them with **custom speed and blend ratios**, and then visualizes both the **time** and **frequency domain** representations.

---

## 👥 Contributors
- **Guhan**
- **Mugil**
- **Adithya**
- **Girisudhan V** *(me)*

---

## 📌 Features

- 🔊 Load and process `.wav` files (vocal & BGM)
- 🌀 Change playback speed for each track
- ⚖️ Blend the two signals with a custom mix ratio
- 📊 Plot:
  - Time-domain waveform
  - Frequency-domain (FFT) spectrum
- 🧪 Check DSP system properties:
  - **Linearity**
  - **Time Invariance**
- 💾 Save mixed audio to a new file
- 🎧 Play the final mix directly from Python

---

## 📂 Project Structure

```
├── audio/
│   ├── voc2.wav            # Vocal input
│   └── bgm2.wav            # Background music input
├── mixed_audio.wav         # Output mix
├── audio_mixer.py          # Main Python script (your provided code)
├── README.md               # This documentation
├── requirements.txt        # Python dependencies
```

---

## 🚀 How to Run

### 1. Install Dependencies

```bash
pip install numpy soundfile sounddevice matplotlib
```

### 2. Run the Code

```bash
python audio_mixer.py
```

> Ensure that `voc2.wav` and `bgm2.wav` are in the same folder or update the path in the code.

---

## 🧪 DSP System Checks

- **Linearity** ✅ / ❌
- **Time Invariance** ✅ / ❌

These checks are performed using:
```python
check_linearity(...)
check_time_invariance(...)
```

Results are printed in the terminal.

---

## 📈 Visual Output

- **Time-domain plots** for vocal, BGM, and mixed output
- **Frequency-domain FFT** for all three signals

### Example Plot:
![Example Time Domain Plot](assets/time_plot_example.png)

---

## 🎧 Output Sample

- Your mixed file will be saved as:
```
mixed_audio.wav
```
- It will auto-play after processing using `sounddevice`.

---

## 💡 Customization

- `speed_vocal = 0.75`  
- `speed_bgm = 1.0`  
- `mix_ratio = 0.7`

Change these values at the top of the script to experiment with different combinations.

---

## 📜 License

This project was built for educational purposes during lab sessions and is open for further improvements or extensions.

---

> Made with ❤️ in the lab by Guhan, Mugil, Adithya, and Girisudhan V.
