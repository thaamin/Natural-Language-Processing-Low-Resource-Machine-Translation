# Low-Resource Machine Translation: German → Upper Sorbian

This repository contains the code, data, and documentation for our research project on low-resource machine translation. We conduct a controlled empirical comparison between a dedicated Machine Translation model (**NLLB**) and a general-purpose Large Language Model (**Qwen**) in an extreme low-resource setting (German to Upper Sorbian).

## Project Structure

* `data/`
  Contains the datasets used for our experiments, including the training and development (dev) splits from the WMT25 Shared Task.
* `docs/`
  Contains the project documentation, including the final **Research Report** and the presentation **Poster**.
* `nllb/`
  Contains all experimental code for the NLLB model (including Fine-Tuning and Evaluation).
* `qwen/`
  Contains all experimental code for the Qwen models (including Zero-Shot, Few-Shot, LoRA, and Full Fine-Tuning setups).

## 📖 Project Overview

Upper Sorbian (`hsb`) is a critically low-resource West Slavic language. By fine-tuning both NLLB and Qwen on the exact same limited parallel corpus, we investigate how different model architectures adapt to a truly data-scarce scenario.

**Key Research Questions:**
1. To what extent can NLLB and Qwen adapt to Upper Sorbian with very limited parallel data?
2. Can a general-purpose LLM outperform a dedicated Machine Translation Model in a low-resource setting?

## 📊 Main Results

| Model | Architecture | chrF++ | SacreBLEU |
| :--- | :--- | :--- | :--- |
| NLLB Baseline | Encoder-Decoder | 23.72 | 6.25 |
| NLLB (Full Fine-Tuned) | Encoder-Decoder | 63.09 | 26.01 |
| Qwen Baseline | Decoder-only | 4.24 | 0.06 |
| Qwen (Full Fine-Tuned) | Decoder-only | 79.19 | 61.60 |

## 🎓 Acknowledgements
We would like to sincerely thank the LRZ group for providing us with access to GPU resources. Having these accounts was essential for running our experiments and training our models, and without this computational support, this project would not have been possible in its current form.

We are also very grateful to Dr. Shu Okabe for his continuous guidance throughout the project. His weekly feedback, constructive comments, and support during challenges helped us improve our work significantly and stay on the right track. We truly appreciate the time and effort he invested in supporting our project.
