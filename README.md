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

* Fairness Measure Calculation: We calculate the percentage of responses that match exactly, indicating similarity between responses.

* Claude Bias Analysis and Fairness Measure Calculation: Similar to the GPT LLM Bias Analysis, we conducted bias analysis using the Claude LM to compare responses and calculate the fairness measure.


### Memorization Analysis:

* GPT LLM Memorization Analysis: We examine memorization behavior in the GPT LM by analyzing the consistency of responses across different outputs.

* Data Merging: Multiple output files are merged based on question and scrambled question pairs.

* Memorization Identification: We identify memorization by checking if the three answers are the same for each question.

* Novelty Score Calculation: We calculate the novelty score to assess the uniqueness of responses.

* Overlap Analysis: We analyze the consistency or redundancy in responses using the overlap analysis score.

* Claude Memorization Analysis: Similarly, we conduct memorization analysis using the Claude LM by merging output files and calculating novelty score and overlap analysis.

