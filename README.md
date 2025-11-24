# Frechet_Audio_Distance
Simple Frechet Audio Distance Test Toolkit


# 🎧 VGGish FAD: Frechet Audio Distance for Audio Evaluation (Minimal)

This project provides a **simple Colab notebook** to compute the **Fréchet Audio Distance (FAD)** between two sets of audio files using **VGGish embeddings**.

> ✅ Perfect for quick evaluation of audio quality: clean vs generated, compressed vs original, or real vs synthesized music.

---

## 🚀 Quickstart (Open in Colab)

Click below to launch the notebook in Colab:

[![Open In Colab]

---

## 📦 What it does

- Loads audio from two folders (real / generated)
- Embeds them with **VGGish**
- Computes mean + covariance for each
- Outputs **Fréchet Audio Distance** (lower = more similar)

---

## 🧪 No data? No problem

If no audio is provided, the notebook automatically generates:
- Clean sine waves (as "real")
- Slightly noisy detuned sine waves (as "generated")

---

## 📋 Dependencies (auto-installed in Colab)

- `torchvggish`
- `librosa`
- `soundfile`
- `tqdm`
- `scipy`
- `resampy`

---

## 🧠 Why use FAD?

FAD is like FID for audio — a perceptual metric that captures statistical similarity between embedding distributions.

Great for:
- Music generation
- Speech enhancement
- Compression quality testing

---

## 📎 Credits

- Based on [frechet-audio-distance](https://github.com/gudgud96/frechet-audio-distance) with simplification for VGGish only.
- Uses [torchvggish](https://github.com/harritaylor/torchvggish)
