# Low-Resource Machine Translation: Upper Sorbian → German

This repository contains code, data processing scripts, and evaluation tools for fine-tuning **NLLB** and **Qwen** models on Upper Sorbian → German translation. The project focuses on **low-resource language translation** using Hugging Face **PEFT/LoRA** and advanced prompting strategies.

## Motivation

Upper Sorbian is a low-resource language with very limited parallel data available for machine translation. Accurate translation is important for preserving minority languages and enabling access to digital content. This project explores **state-of-the-art large language models** for low-resource MT, comparing NLLB fine-tuning and Qwen prompting strategies.

## Project Structure

├── data/
│ ├── train/ # parallel training data
│ └── test/ # parallel testing data
├── experiments/
│ ├── nllb-finetuning/
│ │  ├── train.py          # Fine-tuning script using 
│ │  ├── config.json # Hyperparameters
│ │  └── requirements.txt
│ └── qwen-finetuning/
│    
├── evaluation/
│ ├── nllb-evaluation.py # BLEU, ChrF++, COMET
│ 
├── models/   # Placeholder for models/checkpoints
├── docs/     # Visuals, diagrams, poster PDF
├── README.md
└── LICENSE

