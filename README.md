# Judging Books By Their Cover  

- Welcome to the **Judging Books By Their Cover** repository.
- Using this project, we can tell which genres a book belongs to based on its description.
- This project uses transfer learning and NLP to accomplish the above mentioned task.

## 📝 Description
- Multi-Label Classification refers to the problem of identifying the categories for input data that may belong to multiple categories simultaneously. There may be more than one label for the input data, or there may be no matching labels at all. This approach is excellent for problems like genre classification, where each input text represents a unique blend of different genres. Furthermore, the flexibility of this approach allows us to take care of situations where the input data does not belong to any of the categories in the dataset. This saves us from generating wrong predictions which can be misleading or harmful.
- In this project, we use the ULMFit approach to create a multi-label classifier which can accomplish the aforementioned task.
- We use the **AWD-LSTM** pre-trained language model provided by FastAI and fine-tune it on our dataset. After fine-tuning, we use transfer learning to create the multi-label genre predictor. 

## ⏳ Dataset
- The dataset contains 12 CSV files which contain the most relevant information you can find on a book page.
- Each CSV file represents data from a subgenre of science fiction. For example, *sf_aliens.csv* contains information about books belonging to the genre Science Fiction (Aliens).
- Download the dataset and place it in the main directory.
- Download from [here](https://www.kaggle.com/tanguypledel/science-fiction-books-subgenres?select=sf_alternate_history.csv) .


## :monocle_face: Test this project
To test this project using a friendly GUI, follow these steps:
1. Go to https://mybinder.org/
2. Paste the URL of this repo into Binder’s URL field.
3. Change the File drop-down to instead select URL.
4. In the “URL to open” field, enter “/voila/render/genre_classification_app.ipynb”
5. Click the clipboard button at the bottom right to copy the URL and paste it somewhere safe.
6. Click Launch.
7. Wait a while for the application to launch. Afterwards, you can play around with it and share the link with your friends.

It should look like this:
![binder](https://github.com/mehulfollytobevice/genre_classification/blob/main/pics/binder.PNG)

##  🏽‍ For Genre Prediction, download our model
- For genre prediction, download our model manually: **" multi_genre_classifier.pkl "** from the following place in the repository.
- https://github.com/mehulfollytobevice/genre_classification/tree/main/models
- Download the file and place it into **" ./models/ ".** folder.

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
