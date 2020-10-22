

# Bias in Data - Analysis of Wikipedia Articles

## Goal:

The goal of this assignment is to identify potential sources of bias in a corpus of human-annotated data and describe some implications of those biases.
The corpus you will use is called the Wikipedia Talk corpus, and it consists of three datasets. Each dataset contains thousands of online discussion posts made by Wikipedia editors who were discussing how to write and edit Wikipedia articles. Crowdworkers labelled these posts for three kinds of hostile speech: “toxicity”, “aggression”, and “personal attacks”. Many posts in each dataset were labelled by multiple crowdworkers for each type of hostile speech, to improve accuracy.


## Dataset Sources:

The Datasets used in the analysis can be found below

Toxicity - [Datasets](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Toxicity/4563973)

Aggression - [Datasets](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Aggression/4267550Personal)

Attack - [Datasets](https://figshare.com/articles/dataset/Wikipedia_Talk_Labels_Personal_Attacks/4054689)

## Directory Strucuture:
- code/hcds-a2-data-bias.ipynb -> Main code for analysis
- data/attack/ -> attack dataset
- data/aggression/ -> aggression dataset
- data/toxicity/ -> toxicity dataset

## Requirements:

This analysis was prepared using Python 3.7 running in a Jupyter Notebook environment.

Documentation for Python can be found here: https://docs.python.org/3.7/

Documentation for Jupyter Notebook can be found here: http://jupyter-notebook.readthedocs.io/en/latest/

## Dependencies:

- Pandas

- matplotlib

## Inference
![alt text](https://github.com/Sreejavm/DATA-512-Project-Repo/blob/main/output/output1.png)
- As it can been seen above, toxicity and attack is almost simliar to each other when compared across different age groups, people with different levels of education and their gender
- Majority of the highly attacking/toxic people have bachelors of high school degree. This coincides with the real world data in that people with higher levels of educations are lesser in comparision.
- As seen above, the nearly half the amount of workers belong to 18-30 age group
- Counts of workers decrease with increase in age indicating that workers are compromised mostly of people below 45 years of age
- Since the ratio of male:female is around 3:2, it does not closely represent the real world data in which the ratio is almost 1:1.
- Since age groups are categoried in increments of around 12-15, narrowing down the predictions by a model to tighter bounds of different age groups will be challenging task.
- On a slightly disimiliar note, aggression is high from people in 30-45 age group in comparison with younger audience.
- There is bias is the count of femalte workers in comparision with the count of male workers


![alt text](https://github.com/Sreejavm/DATA-512-Project-Repo/blob/main/output/outpu2.png)
- As it can be seen above female workers are more likely to label a comment as attach than aggression
- Male workers tend to perceive more comments as aggression than female workers
- This bias based on gender in addition to parity in the number of male and female workers will likely result in incorrect labelling of comments. Since male workers are dominating, models are more likely to perceive a comments as aggression based on the above data.
- Bias exists on the dataset with respect of categorization of attacks, aggression or toxicity with respect to gender

## License:

This project code is released under [MIT Licence](https://opensource.org/licenses/MIT).
