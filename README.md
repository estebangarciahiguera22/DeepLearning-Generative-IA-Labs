# DeepLearning Generative AI Labs

This repository contains hands-on Generative AI labs focused on Large Language Models, prompt engineering, fine-tuning, PEFT/LoRA, evaluation metrics, toxicity evaluation, and reinforcement learning with PPO.

# The goal of this repository is to document my practical learning process in modern LLM workflows and connect theory with real implementation using Python, Hugging Face, Google Colab, and open-source models.
------------------------------------------------------
## Repository Structure

``text
DeepLearning-Generative-IA-Labs/
│
├── README.md
│
├── Lab 1/
│   ├── README.md
│   └── Lab_1_Summarize_Dialogue_IA_LLMs_.ipynb
│
├── Lab 2/
│   ├── README.md
│   └── Lab_2_Fine_Tune_Generative_Ai_Model.ipynb
│
└── Lab 3/
    ├── README.md
    └── Lab_3_Fine_Tune_FLAN_T5_with_PPO_and_PEFT_to_Generate_Less_Toxic_Summaries.ipynb
------------------------------------------------------    
## Labs Overview
# Lab 01 — Dialogue Summarization with FLAN-T5

This lab explores dialogue summarization using FLAN-T5 and the DialogSum dataset.

The main focus was to understand how different prompting strategies affect model output without updating the model weights.

# Main topics:

- Dialogue summarization
- Prompt engineering
- Zero-shot inference
- One-shot inference
- Few-shot inference
- Instruction-style prompting
- Generation parameters
- Context window limitations
------------------------------------------------------
## Lab 02 — Fine-Tuning FLAN-T5 with PEFT/LoRA

This lab explores how to fine-tune a language model for dialogue summarization.

It includes full fine-tuning concepts, an educational lightweight fine-tuning workflow, PEFT/LoRA, and ROUGE-based evaluation.

# Main topics:

- Instruction fine-tuning
- Full fine-tuning
- PEFT
- LoRA
- Trainable parameters
- ROUGE evaluation
- Model comparison before and after tuning
------------------------------------------------------
## Lab 03 — PPO + PEFT Detoxification

This lab applies an RLHF-style workflow using PPO and PEFT/LoRA to guide a language model toward generating less toxic summaries.

A RoBERTa-based hate speech classifier was used as a reward model, and the nothate score was used as the positive reward signal.

# Main topics:

- Reinforcement Learning from Human Feedback concepts
- Proximal Policy Optimization
- Reward models
- Toxicity evaluation
- Reference models
- KL divergence
- PEFT/LoRA
- Quantitative and qualitative evaluation
------------------------------------------------------
# Technologies Used
-Python
- Google Colab
- Hugging Face Transformers
- Hugging Face Datasets
- Hugging Face Evaluate
- PyTorch
- PEFT
- LoRA
- TRL
- PPOTrainer
- FLAN-T5
- RoBERTa reward model
- DialogSum dataset
- Learning Outcomes
------------------------------------------------------
# Through these labs, I practiced:

- Building effective prompts for LLM tasks
- Comparing zero-shot, one-shot, and few-shot inference
- Understanding context window limitations
- Fine-tuning models for specific tasks
- Using PEFT/LoRA to reduce trainable parameters
- Evaluating summarization quality with ROUGE
- Using a reward model to guide model behavior
- Applying PPO-style reinforcement learning to LLM outputs
- Measuring toxicity before and after optimization
- Comparing model behavior through quantitative and qualitative evaluation
- Results Summary

------------------------------------------------------
# Lab 01

Prompt engineering improved the quality of generated summaries compared to using the model without a clear instruction.

Few-shot prompting helped guide the model, but too many examples caused context length issues.
------------------------------------------------------
# Lab 02

Fine-tuning changed the behavior of the model and improved ROUGE scores in the lightweight educational experiment.

PEFT/LoRA showed how a model can be adapted by training only a small percentage of its parameters.
------------------------------------------------------
# Lab 03

After lightweight PPO fine-tuning, the mean toxicity score decreased from:

0.00664550035726279

to:

0.006216385716106743

This represented a mean toxicity improvement of:

6.46%

The qualitative comparison also showed that 3 out of 5 examples received a higher nothate reward after PPO.
------------------------------------------------------
## Notes

These labs were completed as part of my Generative AI learning path.

Some notebooks were adapted to run in a personal Google Colab environment. In cases where full training was computationally expensive or course-provided checkpoints were unavailable, lightweight educational alternatives were implemented.

The focus of this repository is educational: understanding the workflow, documenting the process, and demonstrating practical knowledge of modern LLM techniques.
------------------------------------------------------
## Professional Takeaway

This repository demonstrates practical experience with modern Generative AI workflows, including prompt engineering, fine-tuning, parameter-efficient training, evaluation metrics, reward models, and PPO-based reinforcement learning.

It represents part of my AI Engineering portfolio and documents my progression from basic LLM prompting to more advanced model adaptation and alignment techniques.
------------------------------------------------------
## Author 

# Esteban Garcia Higuera




