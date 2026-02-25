# finetune_google-gemma-2B_with_LORA
Fine-tuned Gemma-2B using LoRA with 4-bit quantization on the Abirate/english_quotes dataset. This project demonstrates parameter-efficient supervised fine-tuning with TRL’s SFTTrainer, enabling structured quote–author text generation while keeping GPU memory usage low and training efficient on a single Colab GPU environment.

This project demonstrates parameter-efficient fine-tuning of Gemma-2B using LoRA (Low-Rank Adaptation) with 4-bit quantization on the English Quotes dataset.

The goal is to adapt the base model to generate structured:
Quote: Oustside of a dog, a book is man's.
Author: Mark Twain

🧠 Model & Dataset

Base Model: Gemma by Google

Dataset: Abirate/english_quotes

Fine-tuning Method: LoRA (PEFT)

Quantization: 4-bit NF4 (QLoRA-style training)

Trainer: TRL SFTTrainer

⚙️ Key Features

✅ 4-bit model loading for reduced VRAM usage

✅ LoRA adapters for efficient parameter updates

✅ Structured formatting pipeline

✅ Runs on Google Colab (T4 GPU compatible)

✅ Adapter saving for reuse

pip install transformers datasets accelerate peft trl bitsandbytes
