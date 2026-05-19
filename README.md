# EthiGen: Parameter-Efficient Hate Speech Mitigation

*Developed a Reward-Guided Alignment Pipeline for Non-Hateful Text Generation using RLHF*

## Overview
EthiGen is a project focused on developing a highly efficient, reward-guided alignment pipeline to ensure non-hateful text generation. By leveraging advanced alignment techniques and parameter-efficient fine-tuning, the project achieves a strong balance between text generation quality, semantic relevance, and safety.

## Key Features & Methodology

* **RLHF & PPO Alignment:** Combined Reinforcement Learning with Human Feedback (RLHF) and the Proximal Policy Optimization (PPO) algorithm. This effectively balances safety, coherence, and high-quality generation in a **FLAN-T5** based text generation model.
* **Robust Reward Modeling:** Leveraged a **RoBERTa**-based binary reward model to accurately classify generated text as hate or not hate. 
* **Reward Hacking Mitigation:** Incorporated **KL divergence** to preserve the semantic relevance of the original model and significantly mitigate the risks of reward hacking.
* **Parameter-Efficient Fine-Tuning (PEFT):** Achieved highly efficient training using **LoRA (Low-Rank Adaptation)**. By updating only ~1.4% of the model's total parameters, the project drastically reduces memory usage and enables scalable training even on limited compute resources.

## Tech Stack
* **Base Models:** FLAN-T5 (Generator), RoBERTa (Reward Model)
* **Techniques:** RLHF, PPO, LoRA (Low-Rank Adaptation), KL Divergence penalty
* **Domain:** Natural Language Processing (NLP), AI Safety, Hate Speech Mitigation
