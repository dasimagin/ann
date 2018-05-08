# Answering Neural Network (ANN)

This is a public repo of study project. It's designed for 2nd year students of computer science faculty (HSE + Yandex).

#### AskMe
Intially the project was inspired by work [Ask Me Anything: Dynamic Memory Networks for Natural Language Processing](AskMe.pdf) from Facebook. The article describes dynamic memory network (DMN) which processes input sequences and questions, forms episodic memories, and generates relevant answers. The model was trained on toy Facebook’s bAbI dataset (vocabulary and tasks are dramatically limited).

#### SQuAD
[Stanford Question Answering Dataset](https://rajpurkar.github.io/SQuAD-explorer/) is a new reading comprehension dataset, consisting of questions posed by crowdworkers on a set of Wikipedia articles, where the answer to every question is a segment of text, or span, from the corresponding reading passage. With 100,000+ question-answer pairs on 500+ articles, SQuAD is significantly larger than previous reading comprehension datasets.

#### WikiSearch
Due to this dataset, there is new paper [Reading wikipedia to answer open-domain questions](WikiSearch.pdf).
It's more interesting from practical point of view. This paper proposes to tackle open-domain question answering using Wikipedia as the unique knowledge source. This task of machine reading at scale combines the challenges of document retrieval (finding the relevant articles) with that of machine comprehension of text (identifying the answer spans from those articles).
For search of relevance document authors suggest using rather simple and traditional algorithms, but answering model is based on ANN which is trained on SQuAD dataset.

#### Goals
This project is purely educational. So, students are invited to study technologies and ideas of QA systems which are based on ANN and then learn own model. The long term goal of the project is to implement QA-system, which are based on ANN only.

#### Requirements
Your solution should freely run on ubuntu 14+ and Python 3.4. You also should provide instructions on how to use your application, overview of parameters and code examples of running. A more detailed list of points below:
1. Specify all requirements and version of packages:
 * All python packages
 * All additional deb packages
 * Datasets and additional data that you use
2. prepare.py – script that uploads all essential data, e.g. model parameters. 
3. train.py – script that train your model from scratch.
4. test.py – test scirpts, that evaluates quality of your model (F1-score).
5. demo.py – demo scripts, e.g. it reads from stdin context and question and return answer.
