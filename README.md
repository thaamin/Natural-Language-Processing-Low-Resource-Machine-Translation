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

