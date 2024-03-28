# Prompt-Engineering-Benchmark-Suite
This repo contains a set of evaluation data sets for NLP tasks. It can be used to evaluate prompt engineering techniques on the following use case categories: text generation, commonsense reasoning, arithmetic reasoning, reading comprehension, translation, classification, and code generation. 

It contains 30 hand-picked downstream tasks for each use case category. The original data sets that have been modified were:
- XSum (Text Generation)
- PIQA (Commonsense Reasoning)
- MATH (Arithmetic Reasoning)
- StoryCloze (Reading Comprehension)
- Europarl de-en (Translation)
- AffectiveText (Classification)
- xlcost-text-to-code (Code Generation)

The data sets have been edited to reflect a uniform structure. Each data set contains an unique ID, an input column, optionally two or more solution columns (sol1, sol2, ...), a reference column, and an empty candidate column.

The input column contains information that can be fed to language models that contains instructions for the underlying downstream tasks. If the downstream task is to choose from multiple choices, these are presented in the sol columns. The reference column contains the correct solution. Lastly, the candidate column is always empty and the place where you can paste the cadidate string that the language model did output. 

There are to basic evalutation methods provided, BLEU score and accuracy. 

Please note that all data sets are distributed under different licenses:

XSum, MATH, StoryCloze, and AffectiveText fall under the MIT
