# Fine-Tuning Experiments

Try fine-tuning a small model on a custom dataset to see how behavior changes
compared to prompting a base/instruct model.

## Goals
- Prepare a small, well-labeled dataset for a narrow task.
- Fine-tune (or LoRA fine-tune) a small open model on that dataset.
- Evaluate the fine-tuned model against the base model on held-out examples.

## Possible Tech Stack
- Hugging Face `transformers` + `peft` (for LoRA)
- A small base model (e.g. a distilled or 1-3B parameter model)
- A GPU-enabled environment (local or cloud) for training

## Getting Started
- [ ] Collect/create a small labeled dataset for the target task
- [ ] Pick a base model small enough to fine-tune with available resources
- [ ] Write a training script and run a first short fine-tuning pass
- [ ] Evaluate fine-tuned vs. base model outputs side by side
