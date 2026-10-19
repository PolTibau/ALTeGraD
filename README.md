# ALTeGraD – Advanced Learning for Text and Graph Data

Lab deliverables for the course *Advanced Learning for Text and Graph Data* (ALTeGraD),
part of the Master MVA (Mathématiques, Vision, Apprentissage), 2026-2027.

Author of the answers: **Pol Tibau Rubau**.

## About the course

ALTeGraD is an in-depth exploration of machine learning for text and graph-structured
data. It covers graph representations of text, keyword extraction, modern
Transformer-based language models, attention and sequence-to-sequence architectures,
large language models (LLMs), generative AI for graphs and graph neural networks (GNNs),
with applications such as biology and bioinformatics. The course alternates theory and
practice through lab sessions, and ends with a data challenge on real-world datasets.

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

The lab statements and starter code were provided by the ALTeGraD teaching team.
