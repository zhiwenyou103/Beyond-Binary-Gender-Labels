# Beyond Binary Gender Labels
The official repository for [Beyond Binary Gender Labels: Revealing Gender Bias in LLMs through Gender-Neutral Name Predictions](https://arxiv.org/pdf/2407.05271) 

Name-based gender prediction has traditionally categorized individuals as either female or male based on their names, using a binary classification system. That binary approach can be problematic in the cases of gender-neutral names that do not align with any one gender, among other reasons. Relying solely on binary gender categories without recognizing gender-neutral names can reduce the inclusiveness of gender prediction tasks. We introduce an additional gender category, i.e., "**neutral**", to study and address potential gender biases in Large Language Models (LLMs). We evaluate the performance of several foundational and large language models in predicting gender based on first names only. Additionally, we investigate the impact of adding birth years to enhance the accuracy of gender prediction, accounting for shifting associations between names and genders over time. Our findings indicate that most LLMs identify male and female names with high accuracy (over 80%) but struggle with gender-neutral names (under 40%), and the accuracy of gender prediction is higher for English-based first names than non-English names. The experimental results show that incorporating the birth year does not improve the overall accuracy of gender prediction, especially for names with evolving gender associations. We recommend using caution when applying LLMs for gender identification in downstream tasks, particularly when dealing with non-binary gender labels.

<div align="center">
<img src=./pics/diagram.png width="40%">
</div>

## Datasets
Check the `data` folder for all datasets we used in this paper, including balanced datasets and dynamic gender label datasets. 

## Environment
Please set up the environments as follows: 
```bash
conda create -n <env name> python=3.8.12
pip install transformers pandas openai numpy sentence-transformers datasets
```
