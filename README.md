# SwanNLP @ SemEval-2026-Task-5 : : An LLM-based Framework for Plausibility Scoring in Narrative Word Sense Disambiguation
This repo contains the code and documentation for the SemEval-2026 Task by SwanNLP.

# Authors:
- Deshan Sumanathilaka, Nicholas Micallef, Julian Hough, Saman Jayasinghe
- Department of Computer Science, Swansea University, Wales, UK
- {t.g.d.sumanathilaka, nicholas.micallef, julian.hough, s.j.j.g.galgodagedon}@swansea.ac.uk

## Trained Models

The trained models developed in this project are publicly available on **Hugging Face**.

[![Hugging Face](https://img.shields.io/badge/HuggingFace-Models-yellow?logo=huggingface&logoColor=white)](https://huggingface.co/deshanksuman)
🔗 **Model Hub:** https://huggingface.co/deshanksuman  

## 📊 Fine-tuning Strategies

The table below summarises the mapping between fine-tuning strategies, their training inputs, expected outputs during inference, and the corresponding fine-tuned models.

| **Approach** | **Input** | **Expected Output** | **Fine-tuned Model** |
|--------------|-----------|---------------------|----------------------|
| **Finetuning for Single Annotator Simulation** | Story context, target ambiguous word, candidate sense, and narrative ending. | A plausibility score reflecting the decision of a single human annotator. | deshanksuman/Semeval2026-Qwen-4b-WSD_Reasoning, deshanksuman/Semeval2026-Gemma-4b-WSD_Reasoning |
| **Finetuning for Five Annotator Simulation** | Story context, target ambiguous word, candidate sense, and narrative ending. | An aggregated plausibility score simulating the consensus of five annotators. | deshanksuman/Semeval2026-Qwen-4b-WSD_Reasoning_v2, deshanksuman/Semeval2026-Gemma-4b-WSD_Reasoning_v2 |
| **Finetuning for Single Annotator with Thinking** | Story context, target ambiguous word, candidate sense, narrative ending, correct sense, and reasoning steps. | A plausibility score guided by explicit reasoning steps for a single annotator. | deshanksuman/Semeval2026-Gemma-4b-WSD_Reasoning_v3, deshanksuman/Semeval2026-Qwen-4b-WSD_Reasoning_v3 |
| **Finetuning for Single Annotator with Difficulty Analysis** | Story context, target ambiguous word, candidate sense, narrative ending, with difficulty tag precomputed using the proposed difficulty estimation method. | A plausibility score for a single annotator. | deshanksuman/Semeval2026-Gemma-4b-WSD_Reasoning_v4, deshanksuman/Semeval2026-Qwen-4b-WSD_Reasoning_v4  |


