# 🤮 AI S.L.O.P. Manager - Starter Edition

> **Bypass cloud subscription slop. Run your local AI pipelines offline with a 1-click standalone workspace. Zero Python setup, crash-proof memory control, 100% local power.**

https://github.com/user-attachments/assets/417e462b-f2d7-4bac-aa29-31ae549a5e2d

[![Platform: Windows](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](#)
[![Local-First](https://img.shields.io/badge/Privacy-100%25_Local-brightgreen?style=flat-square)](#)
[![License: Proprietary Wrapper](https://img.shields.io/badge/License-Proprietary_S.L.O.P.-orange?style=flat-square)](#)
[![Backend: ComfyUI](https://img.shields.io/badge/Backend-ComfyUI_&_Ollama-red?style=flat-square)](#)

---

## ⚡ Why Use AI S.L.O.P. Manager?

Running local AI (like ComfyUI and Ollama) usually requires tedious terminal commands, complex environment setups, and constant out-of-memory (OOM) crashes. 

**AI S.L.O.P. Manager** (*Standalone Local Orchestration Platform*) is a native, pre-compiled Windows wrapper that turns your local GPU into a stable, unified creative studio with zero friction.

*   **Instant Local Setup:** No Python or Git required. The integrated installer configures ComfyUI Portable and Ollama automatically on first launch.
*   **Smart VRAM Management:** Automatically orchestrates GPU memory between text (LLM) and image generation tasks to prevent system crashes.
*   **❄️ Hardware Shield (v1.1.1):** Dynamically cooldowns your GPU and flushes VRAM progressively during generation cycles to prevent useless, heavy crash dump files on your system.
*   **Clean Unified Dashboard:** Generate, preview, and manage files without touching terminal screens or complex node-spaghetti graphs.
*   **Total Privacy:** Everything runs on `127.0.0.1`. No telemetry, no cloud API fees, and absolute offline freedom.

---

## 🔮 Currently Included Local Workflows (Starter Edition)

The free version comes pre-configured with three highly optimized local pipelines, ready to run on your local hardware:

### 1. ⚡ ZImage Generation Pipeline (Ultra-Fast)
*   **Powered by:** ZImage Turbo UNET, Qwen 3.4B CLIP, and ZImage VAE.
*   **Capability:** Real-time, lightning-fast generation with highly accurate prompt adherence, optimized for low VRAM consumption.

| ⚡ Generation v01 | ⚡ Generation v02 | ⚡ Generation v03 |
| :---: | :---: | :---: |
| <img width="180" height="180" alt="img_zimage1" src="https://github.com/user-attachments/assets/322d0492-9669-4a3c-af3f-6ba7c9be0f53"/> | <img width="180" height="180" alt="img_zimage2" src="https://github.com/user-attachments/assets/a4b8b5dc-f17b-4860-aece-6b646579f196"/> | <img width="180" height="180" alt="img_zimage3" src="https://github.com/user-attachments/assets/73ce7e17-ab5f-4502-bdbb-cd3e7f47e7e5"/> |

| ⚡ CharacterSheet v01 | ⚡ CharacterSheet v02 | ⚡ CharacterSheet v03 |
| :---: | :---: | :---: |
| <img width="240" height="138" alt="img_zimage_l1" src="https://github.com/user-attachments/assets/5bf73530-fb86-4778-a471-8b08fd4da2a9" /> | <img width="240" height="138" alt="img_zimage_l2" src="https://github.com/user-attachments/assets/dbe54c29-bea3-4b84-acb1-fe30f185984f" /> | <img width="240" height="138" alt="img_zimage_l3" src="https://github.com/user-attachments/assets/b33f71cf-017a-4218-9b32-5ec4d4fa58d0" /> |

### 2. 📸 SDXL Easy Image (Juggernaut XL)
*   **Powered by:** Juggernaut XL v9 RunDiffusion.
*   **Capability:** Highly stable, photorealistic checkpoint. Highly recommended to download first for easy testing.

### 3. 🖌️ Basic Qwen Image Editor (Canvas-Free)
*   **Powered by:** Qwen Image Edit 2511 UNET + Qwen Edit Lightning LoRA.
*   **Capability:** Fast, local image modifications using pure text prompts without complex manual masking.

| 🖼️ Original Input | 🪄 Qwen Edit v01 | 🪄 Qwen Edit v02 |
| :---: | :---: | :---: |
| <img width="240" height="138" alt="img_qwen_orig" src="https://github.com/user-attachments/assets/b510ae85-1e69-4dd8-88bb-30b11746a035" /> | <img width="240" height="138" alt="img_qwen_edit1" src="https://github.com/user-attachments/assets/39369903-81ab-4cc6-877e-98fbd958c6c4" /> | <img width="240" height="138" alt="img_qwen_edit2" src="https://github.com/user-attachments/assets/c9604b66-696c-48bd-b112-bdf790ebcc53" /> |

| 🖼️ Original Input | 🪄 Qwen Edit v01 | 🪄 Qwen Edit v02 |
| :---: | :---: | :---: |
| <img width="200" height="200" alt="img_sdxl_base" src="https://github.com/user-attachments/assets/7ba077ba-de6c-409e-9882-552eb9a0fe1a" /> | <img width="200" height="200" alt="img_qwen_edit3" src="https://github.com/user-attachments/assets/41b29980-f40d-4cf4-ac57-3b4d6389e0ef" /> | <img width="200" height="200" alt="img_qwen_edit4" src="https://github.com/user-attachments/assets/0f9cc8ac-265a-4326-951e-64d7136adb4c" /> |

---

## 🚀 Roadmap & Upcoming Advanced Capabilities

We are actively developing premium standalone tiers to bridge the gap between local 2D generation and production-ready 3D pipeline orchestration:

### 💎 AI S.L.O.P. Manager - 3D Asset Edition (Future Release)
*   **Trellis 2.0 3D Engine:** Native local integration of Microsoft's state-of-the-art **Trellis 2.0 (4B parameter)** image-to-3D framework. Convert any 2D image into textured, arbitrary topology 3D meshes (.glb/.obj) locally.
*   **Asset Expressz (Smart Folder):** Automated directory sorting. Packs your 2D inputs, 3D meshes, prompt text files, and turntable GIFs into structured subdirectories 
*   **Framing Shield:** Automated prompt-injection safety to prevent Trellis from generating cropped or sliced 3D meshes.
*   **GLB/GIF Sync:** Gallery preview utilizing lightweight, animated turntable `.gif` files matched directly with the heavy 3D assets on click.

### 🎬 AI S.L.O.P. Manager - Studio Edition (Future Release)
*   **Local Video Generation Pipeline:** Integration of advanced open-source local video architectures utilizing our smart memory-management engine.

---

## 📦 Getting Started (No Python Required!)

The Starter Edition is compiled as a native Windows C++ binary. You don't need to install Python, Git, or manage Virtual Environments.

1.  Go to the **[Releases](https://github.com/Tamerygo/ai-slop-manager-starterEdition/releases/)** page of this repository.
2.  Download the latest `AI_Slop_Manager_Starter_v1.1.1.zip` package.
3.  Extract the folder anywhere on your local SSD (NVMe recommended).
4.  Run the **`Run_AI_Slop_Manager.bat`** file.
5.  The Setup Wizard will guide you through the initial local engine download.

---

## 🛠️ System Requirements

*   **OS:** Windows 10/11 (64-bit)
*   **GPU:** NVIDIA GeForce (6GB+ VRAM recommended for fast generation / 12GB+ for editing)
*   **Disk Space:** 20GB+ (dependent on downloaded capabilities)

---

## 💎 Support the Local AI Experiments

Love the offline freedom? Support the project to keep local software development alive:

👉 **[Support on Patreon / Buy Me A Coffee]**  
👉 **[Purchase the Advanced Toolchain on Gumroad]**

---

## 🛡️ Enterprise-Grade Security & Safety Guard

We take your system's security and data privacy seriously. **AI S.L.O.P. Manager** implements a strict security layout:

1.  **Zero Executable Risk (100% Safetensors):** We do not use deprecated `.ckpt` (pickle) formats. All graphical workflows are strictly configured to use `.safetensors` files, which are mathematically incapable of executing malicious code or embedding malware.
2.  **Official Hugging Face Direct Pipeline:** Your machine connects directly to official, virus-scanned Hugging Face repositories. No proxy servers, no hidden redirects.

### 🔗 Official Model Sources (Inspect them yourself):
*   **ZImage Turbo UNET:** [Comfy-Org/z_image_turbo](https://huggingface.co/Comfy-Org/z_image_turbo)
*   **Juggernaut XL v9 Checkpoint:** [RunDiffusion/Juggernaut-XL-v9](https://huggingface.co/RunDiffusion/Juggernaut-XL-v9)
*   **Qwen Image Edit 2511 UNET:** [Comfy-Org/Qwen-Image-Edit_ComfyUI](https://huggingface.co/Comfy-Org/Qwen-Image-Edit_ComfyUI)

### ⚖️ Model Licensing Notice
The end-user is solely responsible for complying with the licenses of any downloaded model weights. 
*   Workflows utilizing Apache 2.0 licensed models (e.g. FLUX.2 [klein] 4B) allow for commercial use of the generated assets.
*   Workflows utilizing restricted/non-commercial models (e.g. FLUX.2 [klein] 9B or FLUX.2 [dev]) must be used strictly in accordance with their respective creators' license terms.

## ⚖️ Credits & Open-Source Attributions

AI S.L.O.P. Manager is a proprietary wrapper interface. We stand on the shoulders of giants. The underlying engines executing your generations are open-source masterpieces:

*   **ComfyUI Engine Backend:** (GPLv3 License) – Visual workflow execution API.
*   **Ollama Orchestrator:** (MIT License) – Local LLM runtime.
*   **Gradio UI Framework:** (Apache 2.0 License) – Interactive web-interface components.

*Disclaimer: This software wrapper does not host, bundle, distribute, or sell proprietary model weights. All weights (Llama, Qwen, Flux, SD) are downloaded directly to the user's machine via official APIs and third-party repositories.*
