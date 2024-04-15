# CS521

# Investigating Bias and Memorization in Language Models: An Analysis Across Diverse Question-Answer Datasets

### Description:
This project explores bias and memorization phenomena in language models (LMs) using various question-answer datasets. We analyze how LMs respond to different types of questions, considering factors such as wording variations, demographic references, question structures and jumbling options. The analysis aims to provide insights into the behavior of LMs regarding bias, fairness, and memorization across diverse datasets.

### Source Code Implementation:

#### Data Collection and Preprocessing: We manually built the input datasets by surveying people.

1. allow_forbidden.csv: This dataset contains pairs of questions, with one question presenting a statement in an affirmative stance, while the corresponding "scrambled" question presents a similar statement but from a negative or opposing perspective.

2. demographic_rephrase.csv: The demographic_rephrase dataset consists of survey questions related to various demographic factors, such as location, socioeconomic status, and personal opinions or concerns. Each question is paired with a corresponding scrambled version, altering specific details while maintaining the overall structure and context.

3. jumbled_options.csv: This dataset contains questions where the options for response are presented in a different order compared to the original question.

### Bias Analysis

* GPT LLM Bias Analysis: We utilized the GPT LM (Language Model) to analyze bias in responses. The LM generates responses to survey questions, and we compare the similarity between responses to assess bias.
