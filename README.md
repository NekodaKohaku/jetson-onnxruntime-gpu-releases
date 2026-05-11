# 🚀 ONNX Runtime GPU for Jetson Orin (Python 3.11)

Pre-compiled ONNX Runtime GPU wheels and Docker build scripts for NVIDIA Jetson Orin (JetPack 6.2 / Python 3.11).

This repository provides a custom-built `onnxruntime-gpu` wheel specifically compiled for **NVIDIA Jetson Orin Nano / NX** running **JetPack 6.2** and **Python 3.11**. 

## 📌 為什麼需要這個版本？ (Why this build?)
目前官方與 Jetson AI Lab 並未提供針對 `Python 3.11` + `aarch64` 架構的 ONNX Runtime GPU 預編譯版本。
為了讓 **AivisSpeech Engine** 或其他基於最新 Python 環境的 AI 語音/視覺專案能在 Jetson 邊緣設備上啟用 CUDA 加速，特地編譯此版本供社群使用。

## 📦 環境資訊 (Environment Details)
* **硬體架構 (Architecture)**: `aarch64`
* **目標設備 (Device)**: NVIDIA Jetson Orin Nano / NX
* **作業系統 (OS)**: L4T (JetPack 6.2)
* **Python 版本**: `3.11`
* **ONNX Runtime 版本**: `v1.23.0`

---

## 📥 下載與安裝 (Download & Install)

請直接前往本專案的 **[Releases 頁面](https://github.com/NekodaKohaku/jetson-onnxruntime-gpu-releases/releases)** 下載編譯好的 `.whl` 檔案。

下載後，在你的 Jetson 終端機（或虛擬環境）中執行：
```bash
pip install onnxruntime_gpu-1.23.0-cp311-cp311-linux_aarch64.whl
