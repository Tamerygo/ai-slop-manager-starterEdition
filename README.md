# 🤮 AI Slop Manager - Starter Edition

> **Stop paying ~$20/month for cloud based slop. Run your local AI pipeline completely offline on your own hardware engine.**

[![Platform: Windows](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](https://github.com/)
[![Local-First](https://img.shields.io/badge/Privacy-100%25_Local-brightgreen?style=flat-square)](https://github.com/)
[![License: Proprietary](https://img.shields.io/badge/License-Proprietary_Wrapper-orange?style=flat-square)](https://github.com/)
[![Backend: ComfyUI](https://img.shields.io/badge/Backend-ComfyUI_&_Ollama-red?style=flat-square)](https://github.com/)

**AI Slop Manager** is a standalone, single-executable local workspace designed to wrap, protect, and orchestrate local AI image generation and LLM tasks. It bypasses complex terminal commands and Spaghetti-UI Node setups, giving you a clean, unified control panel on `127.0.0.1`.

---

## ⚡ Key Features (Starter Edition)

*   **Phantom Auto-Bootstrap:** Zero-click installation of ComfyUI Portable and Ollama (if missing) with automated setup.
*   **VRAM Holy Grail Control:** Automated Ollama VRAM flush (`keep_alive: 0`) before launching ComfyUI workflows to prevent out-of-memory (OOM) crashes.
*   **Disk Space Radar:** Integrated Regex-based disk space calculator to block model downloads before you run out of storage.
*   **Zombie Process Exterminator:** Automatic ports cleanup (`8188` & `11434`) on startup and exit to prevent ghost instances.
*   **Live Console Log:** Real-time stdout stream with Windows Encoding Shield, allowing you to see what the generation engines are doing without looking at a black terminal.

---

## 📦 Getting Started (No Python Required!)

The Starter Edition is compiled as a native Windows C++ binary. You don't need to install Python, Git, or manage Virtual Environments.

1. Go to the **[Releases](https://github.com/)** page.
2. Download `AI_Slop_Manager_Starter.zip`.
3. Extract the folder anywhere on your local SSD (NVMe recommended).
4. Run `AI_Slop_Manager.exe`.
5. The Gépész (Installer) will guide you through the initial local setup.

---

## 🛠️ System Requirements

*   **OS:** Windows 10/11 (64-bit)
*   **GPU:** NVIDIA GeForce (6GB+ VRAM recommended) / AMD (experimental local support)
*   **Disk Space:** 20GB+ (for local models and engines)

---

## 💎 Support & Advanced Versions

Love the offline freedom? Support the project on Patreon or Buy Me a Coffee to unlock the **Advanced Toolchain**:

*   **Patreon Supporter Club:** Get early access to stable presets, custom CSS themes, and VIP community Discord.
*   **Advanced Edition (€29 - One-time Purchase):** Unlocks the **Qwen Local Image Editor** (with metadata lineage inheritance) and the **Trellis 3D Mesh Generator** workflow pipeline.

👉 **[Support on Patreon / Buy Me A Coffee]**  
👉 **[Purchase the Advanced Toolchain on Gumroad]**

---

## ⚖️ Credits & Open-Source Attributions

AI Slop Manager is a proprietary wrapper interface. It orchestrates and connects the best open-source AI engines on your machine. We stand on the shoulders of giants:

*   **ComfyUI Backend:** (GPLv3 License) – ComfyUI's core API executes the underlying visual workflows.
*   **Ollama Orchestrator:** (MIT License) – Ollama handles the local LLM runtime and model registry.
*   **Gradio UI Framework:** (Apache 2.0 License) – Powers the reactive web-interface layout.

*Note: This wrapper does not bundle, redistribute, or sell proprietary model weights. All weights (Llama, Qwen, Flux, SD) are downloaded directly to your machine by the installer via official APIs.*