# ALTeGraD – Advanced Learning for Text and Graph Data

Lab deliverables for the course *Advanced Learning for Text and Graph Data* (ALTeGraD),
part of the Master MVA (Mathématiques, Vision, Apprentissage), 2026-2027.

Author of the answers: **Pol Tibau Rubau**.

## Labs

| Notebook | Topic | Main tools |
|---|---|---|
| [`Lab1_Tibau_Rubau_Pol.ipynb`](labs/Lab1_Tibau_Rubau_Pol.ipynb) | **Neural Machine Translation** – sequence-to-sequence model with attention (English → French): greedy and beam-search decoding, analysis of the attention weights | PyTorch, NLTK |
| [`Lab2_Tibau_Rubau_Pol.ipynb`](labs/Lab2_Tibau_Rubau_Pol.ipynb) | **Instruction fine-tuning** – LoRA fine-tuning of Qwen3.5-0.8B-Base on summarization, sampling strategies (temperature, top-p), teaching the model to call tools, bonus fine-tuning in Catalan | Transformers, PEFT, bitsandbytes, Datasets |
| [`Lab3_Tibau_Rubau_Pol.ipynb`](labs/Lab3_Tibau_Rubau_Pol.ipynb) | **Post-training LLMs** – preference optimization with DPO (Qwen3-0.6B on French data) and reinforcement learning with GRPO, with training curves tracked on Weights & Biases | TRL, PEFT, Weights & Biases |

## Running the notebooks

The labs were run on Google Colab with a GPU. Each notebook installs its own
dependencies in its first cells (`!pip install ...`), and Lab 1 downloads its data and
pretrained model at runtime.

Lab 3 logs to Weights & Biases: set your own key before running it, for instance through
the `WANDB_API_KEY` environment variable or by replacing the `<YOUR_WANDB_API_KEY>`
placeholder. Never commit a real key.

## Rights

The lab statements, starter code and pretrained models belong to the ALTeGraD teaching
team. This repository only adds the completed code and the written answers, shared for
reference. For this reason it carries no open-source license: reuse the course material
only as allowed by its authors.
