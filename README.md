# Text-To-Image-Generator
This project implements a full-fledged web application running on Stable Diffusion (via the Diffusers library) that converts natural-language prompts into high-quality images. The app is deployed within Google Colab and served publicly via a secure Cloudflare Tunnel — enabling instant access without needing self-hosted infrastructure.
Key Features

Prompt-driven generation: Users enter a textual prompt (e.g. “a futuristic city at sunset, cinematic lighting”) and receive generated images.

Configurable output: Users can choose the number of images per prompt (1–4), the art style (photorealistic, digital art, oil painting, cartoon, etc.), negative prompts (to avoid unwanted artifacts), diffusion steps, guidance scale, RNG seed, and output format (PNG / JPEG).

Image saving & metadata: All generated images are saved in a time-stamped folder, along with JSON metadata (prompt, full prompt, negative prompt, style, seed, timestamp, model used, etc.).

Downloadable output: Users can view, download, and export images via the web interface (no local setup needed).

GPU-optimized for performance: Utilizes GPU (Tesla T4 on Colab) for acceleration — generation completes in ~30–40 s for first run and ~3–6 s for subsequent runs.

Accessible deployment: Cloudflare Tunnel exposes the app to the web, making it easy to share without complex deployment.

Tech Stack

Python, PyTorch, Diffusers, Transformers

Web UI built with Streamlit

Runtime: Google Colab (GPU-backed)

Tunneling via Cloudflare Tunnel for public access

Image processing via Pillow

Use Cases & Applications

Rapid prototyping of visual ideas & concept art from natural language

Inspiration tool for artists, designers, content creators

Demonstration of generative AI capabilities for educational & portfolio use

Base for building larger systems: concept art generators, story-boarding tools, or art-style transfer pipelines

Why It Matters
This project demonstrates end-to-end mastery — from managing model dependencies to building a responsive UI to deploying a publicly accessible app — all using open-source tools. It showcases not just technical ability in ML modeling and Python programming, but also real-world product thinking and deployment know-how.

Project Status & Next Steps

✅ Fully functional proof-of-concept with SD-v1.5

✅ Handles prompt engineering, custom negative prompts, style presets, multi-format export & metadata logging

🔄 Next enhancements planned: user accounts, prompt history & reuse, image gallery, higher-resolution upscaling, faster models (e.g. SD-Turbo / SD-XL), and persistent storage (cloud or local server) for long-term usage.
