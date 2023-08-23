# Metric-Based In-Context Learning: A Case Study in Text Simplification

This is code for the implementation of the paper "Metric-Based In-Context Learning: A Case Study in Text Simplification."

In the code folder of the repository, you will find the code used to generate data for all of the experiments, including how to generate simplifications from GPT-3 (used in all of our example selection experiments) and our own implementation of KATE-GPT for optimized example selection.

In the output folder of the repository, you will find the results for all experiments that were explained in the paper. The results folder has several sub-folders, for the various experiments that were done. The names of the sub-folders correspond to the method of selecting examples. Each individual folder has its own README with more information on the files and folders inside. 
* BERTPrec - Examples selected using the BERTPrecision metric.
* CR - Examples selected by highest compression ratio.
* FestAbility - SOTA results replicated on the FestAbility dataset during task-transfer experiments
* KATE-GPT - Examples selected with the KATE-GPT algorithm.
* Ordering Examples - We ordered the examples selected by scores in different ways, and this folder includes those results.
* Random Baseline - We perform 3 random baseline experiments, where we randomly select examples without any particular metric in mind.
* SARI - Examples selected using the SARI metric.
* Zero-shot - The model was only given the prompt to simplify, and no examples were provided in this experiment.

In the eval folder, the EASSE reports for each of the experiments are provided. The code and implementation of how to generate the EASSE reports is also provided, so you can replicate our SARI and BLEU scores in our results.

If you have any questions, please feel free to email subhavee2@gmail.com. Thank you!
