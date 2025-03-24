# VLM-Reasoning-Traces

## Overview
This repository contains experimental data comparing reasoning-enabled and base versions of Vision-Language Models (VLMs) for mobile GUI agents. We evaluate two commercial VLMs and their reasoning variants—Claude 3.7 Sonnet and Gemini 2.0 Flash—across three benchmarks: AndroidControl, ScreenSpot (static), and AndroidWorld (interactive).

We include the AndroidControl and ScreenSpot data in this repository.

For more details on the experimental settings and our findings, refer to our paper:
🔗 [**Does Chain-of-Thought Reasoning Help Mobile GUI Agent? An Empirical Study** ](https://arxiv.org/abs/2503.16788)

## News
- **Initial Release**: AndroidControl and ScreenSpot responses from Gemini and Claude models.

## Data Structure
The repository includes responses from four model configurations:
- Gemini Base: `gemini-2.0-flash-001`
- Gemini Thinking: `gemini-2.0-flash-thinking-exp-01-21`
- Claude Base: `claude-3-7-sonnet-20250219`
- Claude Thinking: `claude-3-7-sonnet-20250219`

Files follow the naming convention: `{model_name}_{setup}.jsonl`

### Format
- **AndroidControl**: Each entry contains `episode_id`, `index` (screenshot identifier), and `text` (model output)
- **ScreenSpot**: Each entry contains `filename`, `instruction` (from ScreenSpot), and `text` (model output)
- **Claude Thinking**: Includes additional `thinking` field with the model's reasoning process

---

📢 **If you find this data useful, please consider citing our paper:**
```
@misc{zhang2025doeschainofthoughtreasoninghelp,
      title={Does Chain-of-Thought Reasoning Help Mobile GUI Agent? An Empirical Study}, 
      author={Li Zhang and Longxi Gao and Mengwei Xu},
      year={2025},
      eprint={2503.16788},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2503.16788}, 
}
```
