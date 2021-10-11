# Judging Books By Their Cover  

- This repository contains the code for the **Judging Books By Their Cover** project.
- This project aims to create a multi-label classification system capable of predicting the genres of a book.
- The task mentioned above is accomplished with the help of transfer learning and NLP.

## :question: Problem Statement
In the past decade, online bookstores/ e-commerce websites have taken over traditional bookstores. Most people now order their books online.  In such a scenario, e-bookstores face the challenge of effectively organizing the books according to parameters like genres, ratings, user votes, etc. Each book can belong to multiple genres and appeal to different people. The task is to create a system that can predict the genres of a book based on its description and help in the effective organization of data.  


## 📝 Description
- Multi-Label Classification refers to the problem of identifying the categories for input data that may belong to multiple categories simultaneously. There may be more than one label for the input data, or there may be no matching labels at all. This approach is excellent for problems like genre classification, where each input text represents a unique blend of different genres. Furthermore, the flexibility of this approach allows us to take care of situations where the input data does not belong to any of the categories in the dataset. This saves us from generating wrong predictions which can be misleading or harmful.
- In this project, we use the ULMFit approach to create a multi-label classifier which can accomplish the aforementioned task.
- We use the **AWD-LSTM** pre-trained language model provided by fastai and fine-tune it on our dataset. After fine-tuning, we use transfer learning to create the multi-label genre predictor. 

## ⏳ Dataset
- We use the *Science Fiction Books (10,000+)* dataset from Kaggle.
- The dataset contains 12 CSV files which contain the most relevant information you can find on a book page.
- Each CSV file represents data from a subgenre of science fiction. For example, *sf_aliens.csv* contains information about books belonging to the genre Science Fiction (Aliens).
- Download the dataset and place it in the main directory.
- Download from [here](https://www.kaggle.com/tanguypledel/science-fiction-books-subgenres?select=sf_alternate_history.csv).

## 📝 Description of files
- **Part 1- genre_classification_language_model.ipynb:** In this notebook, we preprocess our data and create a custom language model by fine-tuning the AWD-LSTM pre-trained model provided by fastai.
- **Part 2- genre_classification_eda.ipynb:** In this notebook, we perform EDA to gain a better understanding about the dataset.
- **Part 3- genre_classifier_multi_label.ipynb:** In this notebook, we use the fine-tuned language model created in Part-1 and re-purpose its knowledge to create a multi-label classifier.
- **Part 4- genre_classification_app.ipynb:** Finally, in this part, we put our models to test. We create a *random story generator* and a *multi-label genre predictor* using ipywidgets.

## :hammer_and_wrench: Requirements
* Python 3.5+
* voila
* fastai
* spacy==2.2.4
* packaging
* ipywidgets==7.5.1
* Linux

## Contributors <img src="https://raw.githubusercontent.com/TheDudeThatCode/TheDudeThatCode/master/Assets/Developer.gif" width=35 height=25> 
- Mehul Jain
