# JudgeByCover-
<p align="center">
  "A book recommendation system using Machine Learning — because we all judge by the cover."
<p align="center">
  <img src="Title image.png" width="400"/>
</p>
Reading books is one of my favourite things to do, so I thought — why not try making something useful out of it using machine learning? That's how **JudgeByCover** was born — a fun little web app that recommends books based on what you like!


## 📌 About this project

This is a **Streamlit web application** that recommends similar books based on a user's interest.
You don’t need to type anything — just click on a book title, and the app handles the rest!
It uses a trained ML model to compare books based on certain features and shows you similar ones. Everything runs smoothly in the browser thanks to Streamlit.
### 📺 Demo:

![Demo](tdemo(1).png)
![Demo](tdemo(2).png)
![Demo](tdemo(3).png)


## 🧠 Workflow

1. **Load the data**
2. **Initialize the value of k**
3. For each book, calculate the distance between the user-selected book and all other books (using **Euclidean Distance**)
4. **Sort** the distances
5. **Select top k** nearest neighbors
6. Return the **most similar books** as recommendations

The algorithm behind the model is **K-Nearest Neighbors (KNN)**, implemented using `NearestNeighbors` from `sklearn`.

---

## 📊 Dataset Used

- 📂 [Click here to view/download the dataset](https://www.kaggle.com/datasets/ra4u12/bookrecommendation)
- Contains book titles, authors, ratings, and metadata from multiple sources

## 🧠 Concept used to build the model.pkl file : NearestNeighbors
1. Load the data
2. Initialise the value of k
3. For getting the predicted class, iterate from 1 to total number of training data points
4. Calculate the distance between test data and each row of training data. Here we will use Euclidean distance as our distance metric since it’s the most popular method.
5. Sort the calculated distances in ascending order based on distance values
6. Get top k rows from the sorted array
