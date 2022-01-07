# Multimodal Movie Genre Classification (Text+Image): Prediction on New Data

This notebook shows how to use an already pre-trained model to make predictions on new data. 

### Required files
To run this notebook in Google Colab, you need to download the followings and adjust the paths inside the notebook:
1. [trained model](https://drive.google.com/file/d/1BTmXeu0F9H70TI82xxsLlyy_SnnxsbEN)
2. [dataset to prepare our tokenizer](https://drive.google.com/file/d/1KPC_RYuKNq-viJ7mYjxdNRzfFqgNuBuc) --> filtered from the [original data from TMDB](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [movie posters for prediction](https://drive.google.com/drive/folders/1DnJiYfpNQG1tJdhaMnVot-Vl2A2gHlJ1)

### Input & Output
Input: **Movie Overview (text) & Movie Poster (image)**

Output: **Predicted movie genre**

Example:

<img src="https://imgur.com/3L3vdBa.jpeg" width="600"></img>

### Model
The model used in this notebook is trained following the architectures and codes specified in this [Github repo](https://github.com/dh1105/Multi-modal-movie-genre-prediction).

Some explanations regarding how to train and evaluate the models can be found in this [Medium article](https://towardsdatascience.com/multimodal-deep-learning-to-predict-movie-genres-e6855f814a8a) and the above Github repo.

Basically, the model receives inputs from two modalities, image (movie poster) and text (movie overview). Images are trained using CNN and texts are trained using LSTM. Below is the illustration from the above Medium article.

<img src="https://miro.medium.com/max/4800/1*b4MoSHYfA9U8nPFTXAb4xg.png" width="400"></img>

Illustration from [Source](https://towardsdatascience.com/multimodal-deep-learning-to-predict-movie-genres-e6855f814a8a)
