# Prompt-Engineering-Benchmark-Suite
## Description
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

## Licenses
Please note that the contained data sets fall under different licenses:
### XSUM, MATH, StoryCloze, AffectiveText
XSum, MATH, StoryCloze, and AffectiveText fall under the [MIT License](https://opensource.org/license/mit)

### PIQA
PIQA is distributed under the [AFL 3.0 license](https://opensource.org/license/afl-3-0-php)

### xlcost-text-to-code
xlcost-text-to-code falls under the [CC BY-SA 4.0 Deed](https://creativecommons.org/licenses/by-sa/4.0/ )

### Europarl, StoryClose
Europarl and StoryCloze have no or unknown licenses. Please refer below for original sources.

## Sources

- XSum:
```
@misc{narayan2018dont,
      title={Don't Give Me the Details, Just the Summary! Topic-Aware Convolutional Neural Networks for Extreme Summarization}, 
      author={Shashi Narayan and Shay B. Cohen and Mirella Lapata},
      year={2018},
      eprint={1808.08745},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
- PIQA:
```
@misc{bisk2019piqa,
      title={PIQA: Reasoning about Physical Commonsense in Natural Language}, 
      author={Yonatan Bisk and Rowan Zellers and Ronan Le Bras and Jianfeng Gao and Yejin Choi},
      year={2019},
      eprint={1911.11641},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
- MATH:
```
@misc{hendrycks2021measuring,
      title={Measuring Mathematical Problem Solving With the MATH Dataset}, 
      author={Dan Hendrycks and Collin Burns and Saurav Kadavath and Akul Arora and Steven Basart and Eric Tang and Dawn Song and Jacob Steinhardt},
      year={2021},
      eprint={2103.03874},
      archivePrefix={arXiv},
      primaryClass={cs.LG}
}
```
- StoryCloze:
```
@misc{mostafazadeh2016corpus,
      title={A Corpus and Evaluation Framework for Deeper Understanding of Commonsense Stories}, 
      author={Nasrin Mostafazadeh and Nathanael Chambers and Xiaodong He and Devi Parikh and Dhruv Batra and Lucy Vanderwende and Pushmeet Kohli and James Allen},
      year={2016},
      eprint={1604.01696},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
- Europarl de-en:
```
@inproceedings{inproceedings,
author = {Koehn, Philipp and Och, Franz and Marcu, Daniel},
year = {2003},
month = {01},
pages = {},
title = {Statistical Phrase-Based Translation.},
doi = {10.3115/1073445.1073462}
}
```
- AffectiveText:
```
@inproceedings{strapparava-mihalcea-2007-semeval,
    title = "{S}em{E}val-2007 Task 14: Affective Text",
    author = "Strapparava, Carlo  and
      Mihalcea, Rada",
    editor = "Agirre, Eneko  and
      M{\`a}rquez, Llu{\'\i}s  and
      Wicentowski, Richard",
    booktitle = "Proceedings of the Fourth International Workshop on Semantic Evaluations ({S}em{E}val-2007)",
    month = jun,
    year = "2007",
    address = "Prague, Czech Republic",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/S07-1013",
    pages = "70--74",
}
```
- xlcost-text-to-code:
```
@misc{zhu2022xlcost,
     title = {XLCoST: A Benchmark Dataset for Cross-lingual Code Intelligence},
     url = {https://arxiv.org/abs/2206.08474},
     author = {Zhu, Ming and Jain, Aneesh and Suresh, Karthik and Ravindran, Roshan and Tipirneni, Sindhu and Reddy, Chandan K.},
     year = {2022},
     eprint={2206.08474},
     archivePrefix={arXiv}
}
```
