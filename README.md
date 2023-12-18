# Plant Disease Q&A Chatbot using RNN
This repository contains a Recurrent Neural Network (RNN) model trained on a dataset of question-answer pairs related to plant diseases. The model has been developed to answer queries and provide information about various plant diseases and infections.

## Overview
The RNN-based chatbot leverages a dataset comprising 4000 records of question-answer pairs centered around plant diseases. However, the model has been trained on a subset of 2000 records from this dataset due to constraints. The data used for training has undergone prompt engineering techniques to enhance the chatbot's performance and text generation capabilities.



# Plant Disease Q&A Chatbot using RNN.
This repository contains a Recurrent Neural Network (RNN) model trained on a dataset of question-answer pairs related to plant diseases. The model has been developed to answer queries and provide information about plant diseases and infections.Due to constraints, the model has been trained on a subset of 2000 records from this dataset.

## Dataset Information
The dataset used in this project has been generated using prompt engineering. This dataset comprises 4000 records of question-answer pairs centered around plant diseases.  It consists of several columns, including:

  - User Question: Questions related to plant diseases and issues.
  - Identified Issue: Specific plant diseases or problems identified from the questions.
  - Symptoms: Symptoms associated with the identified plant issues.
  - Management Steps: Steps or solutions to manage or treat the identified plant issues.
  - Response: Answers or information provided in response to the user questions.
  - Preprocessed Columns: Columns with preprocessed text data for various stages in the pipeline, including questions, identified issues, symptoms, management steps, and responses.
  - Additional Columns: Columns indicating length and n-grams for specific text data.

## Code Overview
The provided code is written in Python using TensorFlow and Keras to build and train the RNN model. It involves several pre-processing steps, such as:

  - Text cleaning by converting to lowercase, removing HTML tags, emojis, tokenization, removing stopwords, punctuation, and special characters.
  - Tokenization and sequence padding to prepare the data for model training.
  - Building the RNN model using an Embedding, LSTM, and Dense layer with softmax activation.
  - Training the model on the prepared data using categorical cross-entropy loss and the Adam optimizer.

## How to Use
To use this code:

Ensure you have the necessary libraries installed, particularly TensorFlow, Keras, pandas, numpy, and nltk.
Prepare or have a dataset in a similar format to the provided one, or modify the code to suit your dataset.
Adjust hyperparameters, such as epochs, batch size, and model architecture, according to your requirements.
Train the model by running the code, and make sure to have a GPU if handling a large dataset or longer training times.


## Conversation Loop
The code includes a conversation loop that interacts with the trained model. Users can input queries related to plant diseases, and the model generates responses based on the learned patterns from the training data. The conversation loop allows users to engage with the chatbot until they exit the conversation by typing "exit."

