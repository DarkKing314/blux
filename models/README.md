# 🤖 BLUX Models Directory

Welcome to the **BLUX Models** hub!

This folder catalogs and documents all supported AI models for use across the BLUX ecosystem—whether for code, chat, creativity, or automation.

---

## Supported Model Types

- **Code Models** (e.g., CodeLlama, DeepSeek, StarCoder)
- **Chat/LLM Models** (e.g., Llama, Mistral, Phi)
- **Vision Models** (e.g., CLIP, BLIP, Stable Diffusion)
- **Other Specialized Models** (summarization, search, creative tools)

---

## Adding a Model to BLUX

1. **Download the model:**  
   Download your preferred model from its official source (see below).

2. **Place the model:**  
   Save models in the `blux/models/` directory or configure your `.bluxrc`/config to point to its location.

3. **Register the model:**  
   Add the model to your BLUX config (such as `engines.json` or project-specific model loader).

4. **Use the model:**  
   BLUX will auto-discover supported models at startup, or you can load them via CLI or plugins.

---

## Example Models & Download Links

*(Note: For now, this section lists models you can add; add actual links once downloads are finalized)*

- **Code Models:**
  - [CodeLlama (Meta)](https://github.com/facebookresearch/codellama)
  - [DeepSeek Coder](https://github.com/deepseek-ai/DeepSeek-Coder)
  - [StarCoder](https://huggingface.co/bigcode/starcoder)

- **Chat/LLMs:**
  - [Llama-3 (Meta)](https://ai.meta.com/resources/models-and-libraries/llama-3/)
  - [Mistral](https://mistral.ai/)
  - [Phi-3 (Microsoft)](https://huggingface.co/microsoft/phi-3-mini-4k-instruct)
  - [Gemma (Google)](https://ai.google.dev/gemma)

- **Vision/Multimodal:**
  - [Stable Diffusion](https://github.com/CompVis/stable-diffusion)
  - [CLIP](https://github.com/openai/CLIP)
  - [BLIP](https://github.com/salesforce/BLIP)

---

## Integrating a Model with Plugins

- Create a plugin wrapper for your model, following the [plugin template](../docs/plugins.md).
- Register it in your engine/model config.
- Use BLUX-cA, Quantum, or Lite to call your new engine!

---

## Model Storage Tips

- Use symbolic links if your models are stored elsewhere (e.g., external drives or cloud folders).
- For large models, consider cloud or LAN storage—see [future roadmap](../ecosystem/roadmap.md) for distributed options.

---

## Model Licensing

Always review and comply with each model’s license.  
BLUX does not redistribute proprietary weights—users must download models from official sources.

---

> _Expand your BLUX experience: add, mix, and orchestrate any AI model you like!_
