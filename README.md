# 🤮 AI Slop Manager - Starter Edition

>  **Bypass cloud subscription slop. Run your local AI pipelines offline with a 1-click workspace. Zero Python setup, crash-proof memory control, 100% local power.**

[![Platform: Windows](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](#)
[![Local-First](https://img.shields.io/badge/Privacy-100%25_Local-brightgreen?style=flat-square)](#)
[![License: Proprietary Wrapper](https://img.shields.io/badge/License-Proprietary_Wrapper-orange?style=flat-square)](#)
[![Backend: ComfyUI](https://img.shields.io/badge/Backend-ComfyUI_&_Ollama-red?style=flat-square)](#)

---

## ⚡ Why Use AI Slop Manager?

Running local AI (like ComfyUI and Ollama) usually requires terminal commands, custom environment setups, and constant out-of-memory (OOM) crashes. **AI Slop Manager** is a native, pre-compiled Windows wrapper that turns your local GPU into a stable, unified creative studio with zero friction.

*   **Instant Local Setup:** No Python or Git required. The integrated installer configures ComfyUI Portable and Ollama automatically on first launch.
*   **Smart VRAM Management:** Automatically orchestrates GPU memory between text (LLM) and image generation tasks to prevent system crashes.
*   **Clean Unified Dashboard:** Generate, preview, and manage files without touching terminal screens or complex node-spaghetti graphs.
*   **Total Privacy:** Everything runs on `127.0.0.1`. No telemetry, no cloud API fees, and absolute offline freedom.

## 🔮 Currently Included Local Workflows (Starter Edition)

The free version comes pre-configured with three highly optimized local pipelines, ready to run on your local hardware:

1.  **⚡ ZImage Generation Pipeline (Ultra-Fast):**
    *   *Powered by:* ZImage Turbo UNET, Qwen 3.4B CLIP, and ZImage VAE.
    *   *Capability:* Real-time, lightning-fast generation with highly accurate prompt adherence, optimized for low VRAM consumption.
2.  **📸 SDXL Easy Image (Juggernaut XL):**
    *   *Powered by:* Juggernaut XL v9 RunDiffusion.
    *   *Capability:* Photorealistic, studio-quality, high-fidelity local photography generation with rich lighting and textures.
3.  **🖌️ Basic Qwen Image Editor (Canvas-free):**
    *   *Powered by:* Qwen Image Edit 2511 UNET + Qwen Edit Lightning LoRA.
    *   *Capability:* Fast, local image modifications using pure text prompts without complex manual masking.

---

## 🚀 Roadmap & Upcoming Advanced Capabilities

I am actively developing the **Advanced Toolchain (€29 Tier)** to bridge the gap between local 2D generation and production-ready 3D pipeline orchestration:

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
3.  Extract the folder anywhere on your local SSD.
4.  Run `Run_AI_Slop_Manager.bat`.
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
