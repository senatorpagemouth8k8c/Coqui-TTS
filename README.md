# OmniGen-Local

> **A unified, offline-first AI studio for text, image, audio, and video generation — all on your machine.**  
> No internet. No telemetry. No external dependencies after setup.

OmniGen-Local is a self-contained desktop application that brings **multimodal generative AI** to your personal computer. Write stories, paint images, compose music, and animate scenes — entirely offline, with full control over models, data, and outputs.

<p align="center">
  <img src="https://placehold.co/400x225/0f172a/ffffff?text=Text+Output%3A+A+poem+about+autumn" width="23%"/>
  <img src="https://placehold.co/400x225/1e293b/ffffff?text=Image%3A+Cyberpunk+market+at+night" width="23%"/>
  <img src="https://placehold.co/400x225/020617/ffffff?text=Audio%3A+Piano+melody+in+C+minor" width="23%"/>
  <img src="https://placehold.co/400x225/1e1b4b/ffffff?text=Video%3A+Leaves+falling+in+slow+motion" width="23%"/>
</p>

---

## Philosophy

OmniGen-Local is built on three principles:

- **Local-first**: All computation happens on your device.  
- **Modular**: Swap models, pipelines, and modalities independently.  
- **Transparent**: Every model is open-weight; every output is yours.  

This is not a product. It is a **workspace for creators, researchers, and tinkerers** who value sovereignty over convenience.

---

## Capabilities by Modality

### 📝 Text
- Conversational AI (7B–13B parameter models)
- Code generation, summarization, translation
- Local LLMs: Llama 3, Mistral, Phi-3 (GGUF format)

### 🖼️ Image
- Text-to-image (Stable Diffusion 1.5/2.1/SDXL)
- Inpainting, outpainting, image-to-image
- LoRA, ControlNet, Tiled Diffusion support

### 🎧 Audio
- Text-to-speech (Coqui TTS, Bark-lite)
- Music generation (AudioLDM-2, MusicGen-small)
- Voice cloning (opt-in, requires local dataset)

### 🎥 Video
- Text-to-video (ZeroScope, ModelScope)
- Image-to-video (AnimateDiff lightweight)
- 2–8 second clips at 256×256 or 512×512

All models run **offline**. No automatic downloads.

---

## Application Interface

<p align="center">
  <img src="https://placehold.co/900x500/0f172a/64748b?text=OmniGen-Local+UI+-+Tabbed%2C+Dark%2C+Unified" width="90%"/>
</p>

- **Tab-based workspace**: switch between modalities seamlessly  
- **Unified prompt bar** with syntax highlighting  
- **Model selector**: choose from local checkpoints  
- **Output panel**: preview, export, or iterate  
- **Metadata panel**: view full generation parameters  
- **Cross-modal chaining**: e.g., generate text → image → video  

Exports: TXT, PNG, MP3, MP4, WAV, GIF — all to your `Documents/OmniGen-Local/` folder.

---

## Performance & Hardware

| Modality | Hardware        | Example Task                     | Time     |
|----------|-----------------|----------------------------------|----------|
| Text     | RTX 4070        | 512 tokens @ 45 tok/s            | ~11 sec  |
| Image    | M2 Max          | 1024×1024 SDXL (30 steps)        | ~5.2 sec |
| Audio    | i7-13700        | 10 sec music clip                | ~18 sec  |
| Video    | RTX 3060        | 4-sec 512×512 clip               | ~2.1 min |

Optimizations:  
- GPU: CUDA (NVIDIA), MPS (Apple), ROCm (AMD)  
- CPU: AVX2, quantized models (GGUF, safetensors)  
- Memory: automatic offloading for large models

---

## Download

Pre-built binaries (no Python required):

- **Windows**: [`OmniGen-Local-v1.0-win-x64.exe`](https://example.com)  
- **macOS**: [`OmniGen-Local-v1.0-mac-universal.dmg`](https://example.com)  
- **Linux**: [`OmniGen-Local-v1.0-linux-x64.AppImage`](https://example.com)

> All builds are code-signed. SHA256 checksums provided.

---

## Ethical Use

You must not use OmniGen-Local to:
- Generate synthetic media of real individuals without consent  
- Create harmful, illegal, or deceptive content  
- Circumvent copyright or privacy protections  
- Automate disinformation  

Model weights are subject to their original licenses (e.g., **Llama Community License**, **OpenRAIL-M**). Review each before use.

---

## Technical Foundation

- **Text**: llama.cpp + GGUF  
- **Image**: Diffusers + Automatic1111-compatible pipelines  
- **Audio**: Transformers + torchaudio  
- **Video**: Text2Video-Zero + AnimateDiff-lite  
- **UI**: Custom Electron + React (compiled to native)  
- **License**: **Code — MIT** | **Models — as per source**

---

## Support & Contribution

- Questions? → [Discussions](https://github.com/your-username/OmniGen-Local/discussions)  
- Bugs? → [Issues](https://github.com/your-username/OmniGen-Local/issues)  
- Want to add a model? → Pull requests welcome  

We value **honesty about limitations** as much as technical ambition.

---

**OmniGen-Local**: One studio. All modalities. Your machine. Your control.
