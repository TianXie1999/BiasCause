# BiasCause

This is the dataset and code for BiasCause framework.

#### BiasCause Dataset.xlsx 

This file contains: 

- all questions
- answers to the questions by 4 different LLMs in 3 rounds of experiments (All_answers_1 to All_answers_3)
- extracted causal graphs of the answers by 4 different LLMs in 3 rounds of experiments (All_answers_1 to All_answers_3)
- labeling of answers and the causal reasoning

#### Code folder

This folder contains code to generate answers to the questions, evaluate the answer correctness, and classify causal labeling. Note that we delete some code related to confidential google environment, but the workflow (including prompts) has been demonstrated in detail in both our paper and the code folder.

- Gemini_batch_prediction.ipynb: code to generate batch prediction using Vertex AI and Gemini
- Claude_batch.ipynb: code to generate batch prediction using Vertex AI and Claude
- Data_and_gemma_inference.ipynb: code to generate answers using an endpoint of Gemma 2
- Autorater_evaluation.ipynb: code to prepare data for autorater evaluation
- Evaluation_results_all_models.ipynb: code to analyze the evaluation results

