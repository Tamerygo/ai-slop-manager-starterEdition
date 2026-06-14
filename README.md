# 🤮 AI Slop Manager - Starter Edition

> **Stop paying $20/month for cloud-censored subscription slop. Run your local AI pipelines offline with 1-click. Crash-proof VRAM control, zero Python setup, pure local power on `127.0.0.1`.**

[![Platform: Windows](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](#)
[![Local-First](https://img.shields.io/badge/Privacy-100%25_Local-brightgreen?style=flat-square)](#)
[![License: Proprietary Wrapper](https://img.shields.io/badge/License-Proprietary_Wrapper-orange?style=flat-square)](#)
[![Backend: ComfyUI](https://img.shields.io/badge/Backend-ComfyUI_&_Ollama-red?style=flat-square)](#)

---

## 🛑 The Anti-Slop Manifesto

Tired of complex terminal setups, out-of-memory errors, and paying recurring fees for censored cloud models? Run your own AI Studio locally, with zero friction. **AI Slop Manager** is a standalone, compiled C++ binary that wraps, protects, and orchestrates local generative engines directly on your GPU.

*   **Zero-Click Bootstrap:** No Python, no Git, no command-line spaghetti. One double-click, and you are ready.
*   **Smart VRAM Shield:** Automatically flushes Ollama memory before launching ComfyUI to prevent out-of-memory (OOM) crashes.
*   **100% Offline & Private:** Your prompts, your images, your data. Everything stays on your local machine.
*   **Disk Space Radar:** Calculates model sizes before downloading. Prevents incomplete downloads and bricked SSDs.
*   **Built-in Exterminator:** Kills zombie background processes on ports `8188` and `11434` with a single click.

---

## 🛠️ What Can You Actually Do With the Starter Edition?

The **Starter Edition** is a fully functional, production-ready local orchestrator. It is engineered to solve the most painful friction points of running local Generative AI:

### 1. 🚀 Zero-Configuration One-Click Setup
*   **Phantom Auto-Bootstrap:** You don't need to manually download ComfyUI, install Python, or configure Ollama. On the first launch, the app automatically pulls the official silent installers, extracts the Portable environments using a built-in 7-zip backend, and boots everything up.
*   **Dynamic Path Management:** Want to use an external SSD for your heavy models? You can customize your installation paths inside the UI. The manager dynamically writes ComfyUI's `extra_model_paths.yaml` in the background.

### 2. 🧠 Smart VRAM & Engine Orchestration (Zero-OOM)
*   **The VRAM Holy Grail:** If you try to run ComfyUI generation while an Ollama LLM is holding your GPU memory, your system will crash. The Starter Edition automatically intercepts the generation call, forcefully flushes the Ollama VRAM (`keep_alive: 0` API call), sleeps for 1 second to let your GPU clear, and then safely executes your ComfyUI workflow.
*   **Automatic LLM Detection & Fallback:** The system scans your local Ollama registry. It automatically routes the "Director" role to the best available Gemma model, and the "Mechanic/Coder" role to Qwen. If Qwen is missing, the Director automatically steps in to handle both roles, preventing any `404 Not Found` API crashes.

### 3. 🛡️ Absolute System Stability & Process Control
*   **Zombie Process Exterminator:** When local AI servers crash, they often leave phantom processes locked on ports `8188` (ComfyUI) and `11434` (Ollama). The manager forcefully kills these ghost processes on startup and shutdown using native OS signals.
*   **Active Live Console Log:** Watch ComfyUI's console output live inside the Gradio UI. Built with a Windows Encoding Shield (`errors="replace"` and `PYTHONUNBUFFERED=1`), it updates progressively so you always know what your machine is doing without looking at a black terminal screen.
*   **Disk Space Radar:** Before downloading any heavy 20GB+ capability, the built-in space checker parses the model sizes using regex, compares them with your actual drive space, and safely blocks the download if your disk is about to get bricked.

### 4. 📸 Local Image Generation & Smart Lineage
*   **Capability-Driven Feature Manager:** You don't manage cryptic model filenames. You install and delete "Capabilities" (e.g., *Ultra-Fast Image Generator*, *Easy Image*). Want to free up space? Uninstalling a capability deletes all its sub-components from your drive with one click.
*   **Local Preset Manager:** Save your favorite resolutions, styles, prompts, negative prompts, and sliders into a local `presets.json` database. Load or delete them on the fly.
*   **Bypassing the Gradio Sandbox (Path-Hack):** Web browsers hide the true paths of your uploaded images. The custom "Send to Input 1" button lets you pass the exact, unmasked local path to the backend via a hidden State manager.
*   **Data Lineage (Metadata Inheritance):** When uploading an image to modify it, the pipeline reads the `.txt` sidecar metadata from the source file, extracts the `ORIGINAL POSITIVE` and `NEGATIVE` prompts, and appends your edits on top of them, preserving the creative lineage.
*   **Nuclear Gallery Grid CSS:** Override Gradio's standard layouts. Features a responsive CSS-grid with sliders to dynamically change columns (1 to 8), scale lightbox thumbnails in real-time, and set maximum loaded files (1 to 500) without crashing your browser.
*   **Sequential Batch Seed Injection:** Generate multiple images in a loop safely. The pipeline dynamically injects a unique 32-bit integer seed for every batch iteration to bypass ComfyUI caching, updating the gallery progressively.

---

## 🔮 Currently Included Local Workflows (Starter Edition)

The free version comes pre-configured with three highly optimized local pipelines, ready to run on your local hardware:

1.  **⚡ ZImage Generation Pipeline (Ultra-Fast):**
    *   *Powered by:* ZImage Turbo UNET, Qwen 3.4B CLIP, and ZImage VAE.
    *   *Capability:* Real-time, lightning-fast generation with highly accurate prompt adherence, optimized for low VRAM consumption.
2.  **📸 SDXL Photographic Studio (Juggernaut XL):**
    *   *Powered by:* Juggernaut XL v9 RunDiffusion.
    *   *Capability:* Photorealistic, studio-quality, high-fidelity local photography generation with rich lighting and textures.
3.  **🖌️ Basic Qwen Image Editor (Canvas-free):**
    *   *Powered by:* Qwen Image Edit 2511 UNET + Qwen Edit Lightning LoRA.
    *   *Capability:* Fast, local image modifications using pure text prompts without complex manual masking.

---

## 🚀 Roadmap & Upcoming Advanced Capabilities

We are actively developing the **Advanced Toolchain (€29 Tier)** to bridge the gap between local 2D generation and production-ready 3D pipeline orchestration:

*   **🎨 Advanced Qwen Image Edit Workflow:**
    *   Highly precise local canvas manipulation, advanced selective inpainting, multi-angle consistency controls, and deep style transfer leveraging the full Qwen-VL vision pipeline.
*   **🧊 Trellis 2 3D Asset Generator (Microsoft TRELLIS.2 Integration):**
    *   Native local wrapper for Microsoft's state-of-the-art **Trellis 2.0 (4B parameter)** image-to-3D framework.
    *   Turn any generated local 2D image into a high-fidelity, fully textured, arbitrary topology 3D mesh (.glb/.obj) with complete PBR materials (Base Color, Metallic, Roughness) in seconds on consumer-grade GPUs.

---

## 📦 Getting Started (No Python Required!)

The Starter Edition is compiled as a native Windows C++ binary. You don't need to install Python, Git, or manage Virtual Environments.

1.  Go to the **[Releases](https://github.com/)** page of this repository.
2.  Download the latest `AI_Slop_Manager_Starter_vX.Y.Z.zip` package.
3.  Extract the folder anywhere on your local SSD (NVMe highly recommended).
4.  Run `app_starter.exe`.
5.  The Setup Wizard will guide you through the initial local engine download.

---

## 🛠️ System Requirements

*   **OS:** Windows 10/11 (64-bit)
*   **GPU:** NVIDIA GeForce (6GB+ VRAM recommended for fast generation / 12GB+ for editing)
*   **Disk Space:** 20GB+ (dependent on downloaded capabilities)

---

## 💎 Support the Local AI Resistance

Love the offline freedom? Support the project to keep local software development alive:

👉 **[Support on Patreon / Buy Me A Coffee]**  
👉 **[Purchase the Advanced Toolchain on Gumroad]**

---

## ⚖️ Credits & Open-Source Attributions

AI Slop Manager is a proprietary wrapper interface. We stand on the shoulders of giants. The underlying engines executing your generations are open-source masterpieces:

*   **ComfyUI Engine Backend:** (GPLv3 License) – Visual workflow execution API.
*   **Ollama Orchestrator:** (MIT License) – Local LLM runtime.
*   **Gradio UI Framework:** (Apache 2.0 License) – Interactive web-interface components.

*Disclaimer: This software wrapper does not host, bundle, distribute, or sell proprietary model weights. All weights (Llama, Qwen, Flux, SD) are downloaded directly to the user's machine via official APIs and third-party repositories.*