# Hi, I'm Tobias 👋

Pentester and malware analyst from Basel, Switzerland. By day I look for the holes in other people's systems. In the evenings I build my own: a home lab that runs AI locally, with agents that do real work and an eye on how to keep them safe.

## What's running in my lab

| Machine | What it does |
| --- | --- |
| **2x NVIDIA DGX Spark** (GB10, 128 GB each, linked over ConnectX-7) | GLM-5.3-Flash, tensor-parallel across both, the main model behind my agents |
| **Windows PC with an RTX 5090** | vision (Qwen3.8-27B), OCR at scale (GLM-OCR, PaddleOCR-VL), image generation with ComfyUI, image-to-3D for my 3D printer |
| **Mac mini M4 Pro** | the conductor: Hermes Agent with several profiles, Hindsight as shared long-term memory, speech in and out (Whisper, Qwen3-TTS on MLX), a local Qwen fallback |
| **Synology NAS** | sync, backups, n8n workflows |
| **Raspberry Pi 5 + Hailo** | Home Assistant and camera detection |

Cloud models (Claude, Codex, Mistral) do the planning and the reviews. Bulk work and anything private stay on my own hardware.

## How I like to work

- **Measure, don't guess.** Every number gets a source and a stated limit.
- **Security first.** Agents get the least privilege they need, secrets stay out of repos, private data stays local.
- **Make it traceable.** If I can't explain later what changed and why, it isn't done.

## Where I'm heading

- An agent system that handles most of my routine work, so I only step in where a decision really matters.
- A write-up about once a month: benchmarks on the Sparks and the RTX 5090, agent setups, and security for AI tooling.
- Learning by building, and making it easier for others to do the same.

## Latest

- 📊 **[GLM-5.3-Flash on 2x DGX Spark: vLLM vs. TensorFold](https://github.com/Tobiasris/glm-5.3-flash-dgx-spark-benchmark)**: five configurations measured on the same pair. TensorFold was up to 2x faster, and I split the gain into engine, drafter and quantization. Also on [Hugging Face](https://huggingface.co/datasets/Tobiasris/glm-5.3-flash-dgx-spark-benchmark) and in the [NVIDIA forum](https://forums.developer.nvidia.com/t/389221).

## Say hi

I'm always happy to compare notes. If you run similar hardware, have numbers that contradict mine, or spot a mistake anywhere in my work, please tell me. Open an issue, comment on Hugging Face or reply in the NVIDIA forum. I'd honestly like to hear it, and I'll fix and credit whatever turns out to be wrong.

[tobiasris.ch](https://tobiasris.ch) · [Hugging Face](https://huggingface.co/Tobiasris) · [NVIDIA Developer Forum](https://forums.developer.nvidia.com/u/ristobias)
