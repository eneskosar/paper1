# An Empirical Study of Fine-Tuning Effectiveness Across Transformer Architectures for Logical Reasoning

This repository accompanies our short empirical study on supervised fine-tuning 
for logical reasoning across different transformer architectures.

We evaluate encoder-only, decoder-only, and encoder–decoder models under 
controlled fine-tuning settings on the FOLIO benchmark, aiming to understand 
their practical performance limits when properly optimized.

---

## Repository Structure

- `1encoders_ft.ipynb`  
  Fine-tuning experiments for encoder-only models  
  (e.g., BERT, RoBERTa, DeBERTa, ELECTRA).

- `2decoders_ft (1).ipynb`  
  Fine-tuning experiments for decoder-only models  
  (e.g., LLaMA-style, Qwen-style models).

- `3encoderdecoder.ipynb`  
  Fine-tuning experiments for encoder–decoder models  
  (e.g., T5 / Flan-T5).

- `3encoderdecoder2 (12).ipynb`  
  Extended experiments and additional configurations 
  for encoder–decoder models.

---

## Experimental Setup

- Dataset: FOLIO (First-Order Logic reasoning benchmark)
- Training: Supervised fine-tuning
- Evaluation: Accuracy on entailment-style premise → conclusion classification
- Models span encoder-only, decoder-only, and encoder–decoder families.

All experiments are implemented using HuggingFace Transformers and 
standard fine-tuning pipelines.

---

## Key Goal

To provide a systematic empirical comparison of how different transformer 
architectural families respond to supervised fine-tuning for logical reasoning.

Rather than proposing a new architecture or solver pipeline, 
this work investigates the effectiveness and limits of standard fine-tuning 
when carefully applied across model types.

---

## Notes

Notebooks are designed to be run independently.
Please configure:

- Model names
- GPU settings
- Dataset paths

before execution.

---

## Citation

If you find this repository useful in academic work, 
please cite our accompanying paper (details to be added).
