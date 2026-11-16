# Hi, I'm Tobias 👋

Pentester and malware analyst from Basel, Switzerland. By day I look for the holes in other people's systems. In the evenings I build my own: a home lab that runs AI locally, agents that do real work, and more and more hardware that I design, print and wire up myself.

I love learning new things, and I learn best by building them, breaking them and measuring what happened.

## What's running in my lab

| Machine | What it does |
| --- | --- |
| **2x NVIDIA DGX Spark** (GB10, 128 GB each, linked over ConnectX-7) | GLM-5.3-Flash, tensor-parallel across both, the main model behind my agents |
| **Windows PC with an RTX 5090** | vision, OCR at scale, image generation with ComfyUI, image-to-3D for the printer |
| **Mac mini M4 Pro** | the conductor: [Hermes Agent](https://github.com/NousResearch/hermes-agent) with several profiles, [Hindsight](https://github.com/vectorize-io/hindsight) as shared long-term memory, speech in and out, a local fallback model |
| **Arduino VENTUNO Q** | edge AI on a small board with its own NPU, my playground for running models close to sensors |
| **Raspberry Pi** | [Home Assistant](https://www.home-assistant.io) and camera detection |
| **A NAS** | sync, backups, [n8n](https://n8n.io) workflows |

## The workshop

Software is only half of it. I'm teaching myself how to build hardware: enclosures, mounts and small devices, from the first sketch to the finished part.

- **[Bambu Lab](https://bambulab.com) H2C** for 3D printing, fed straight from the lab (image → 3D model → print)
- **[Arduino](https://www.arduino.cc)** boards and sensors for the electronics
- CAD (Fusion) for the parts that need to fit on the first try (they rarely do)

## The AI I work with

Cloud models do the planning and the reviews. Bulk work and anything private stay on my own hardware.

| | Used for |
| --- | --- |
| [Claude](https://www.anthropic.com/claude) (Anthropic) | planning, hard decisions, code review |
| [Codex](https://openai.com/codex) (OpenAI) | coding tasks and a second opinion |
| [Mistral](https://mistral.ai) | coding with Vibe, reviews |
| [GLM](https://huggingface.co/zai-org) (Z.ai) | local main model on the Sparks |
| [vLLM](https://github.com/vllm-project/vllm), [llama.cpp](https://github.com/ggml-org/llama.cpp), [Ollama](https://ollama.com) | serving models locally |

## How I like to work

- **Measure, don't guess.** Every number gets a source and a stated limit.
- **Security first.** Agents get the least privilege they need, secrets stay out of repos, private data stays local.
- **Make it traceable.** If I can't explain later what changed and why, it isn't done.

## Where I'm heading

- An agent system that handles most of my routine work, so I only step in where a decision really matters.
- A write-up about once a month: benchmarks on the Sparks and the RTX 5090, agent setups, hardware builds and security for AI tooling.
- Learning by building, and making it easier for others to do the same.

## Latest

- 📊 **[GLM-5.3-Flash on 2x DGX Spark: vLLM vs. TensorFold](https://github.com/Tobiasris/glm-5.3-flash-dgx-spark-benchmark)**: five configurations measured on the same pair. TensorFold was up to 2x faster, and I split the gain into engine, drafter and quantization. Also on [Hugging Face](https://huggingface.co/datasets/Tobiasris/glm-5.3-flash-dgx-spark-benchmark) and in the [NVIDIA forum](https://forums.developer.nvidia.com/t/389221).

## Say hi

I'm always happy to compare notes. If you run similar hardware, have numbers that contradict mine, or spot a mistake anywhere in my work, please tell me. Open an issue, comment on Hugging Face or reply in the NVIDIA forum. I'd honestly like to hear it, and I'll fix and credit whatever turns out to be wrong.

[tobiasris.ch](https://tobiasris.ch) · [Hugging Face](https://huggingface.co/Tobiasris) · [NVIDIA Developer Forum](https://forums.developer.nvidia.com/u/ristobias)
