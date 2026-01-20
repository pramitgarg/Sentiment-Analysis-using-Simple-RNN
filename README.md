# Sentiment-Analysis-using-Simple-RNN
This project shows the simple RNN used to do text classification of movie review's given by IMDB and using streamlit to display and then deploy it on Streamlit Cloud.

<img width="1018" height="600" alt="Screenshot 2026-01-19 at 3 08 42 PM" src="https://github.com/user-attachments/assets/d76f7cb9-f1dd-4521-8166-44eda0277174" />


In this Project, we have download the datasets from the tensorflow and build the RNN model. Here are the steps taken to execute this project : 
1. Creating the Gituhb repo and clone the repo on VS code on my local system.
   
2. Creating an virtual environment with [ python -m venv .venv ] and activate the environment by source  activate/bin/.venv. Downloading libraries like ipykernel, tensorlfow, keras etc in the requirements.txt file and installing all the libraries through pip install -r requirements.txt.

3. Created Embedding.ipynb file and converted a sample text into embeddings. The steps involved in converting text into embeddings are:                                     
   A. First, we are going to set the vocabulary words so that there is a limited word from the dataset which is converted and on which model is trained so that the model can be more effecient and fast.                                                                                                                                              
   B. Using one_hot technique which converts the words [ categorical variables ] into Vectors [ binary format]                                                           
   C. We import libraries like Embedding, Pad_sequence, sequential where Pad_sequence fills the 0's to pre or post in the line where the words are less than the limit set for each line.                                                                                                                                                                             
   D. Feature prepresentation dimenstion are going to be set so that each word can be compared with the dimensions set.                                                               
   E. Using Sequential model technique in order to create RNN model because Sequential processing ensures that instructions are executed in a predictable and ordered manner, allowing for reliable and consistent results.     

4. Creating RNN Model in SimpleRNN.ipynb file. Steps Taken to build the model :                                   
   A. We are going to download the IMDB movie Reviews Dataset from the library Tensorflow.keras.datasets import db. Because it is a big dataset so we are not going to import limited data with max_features from the dataset so that we can train the model more effeciently.     B. Once we have loaded the dataset and split the data into train & test data, then we are going to import sequence from tensorflow.keras and do the pad_sequencing of the sentence and set the number of words in a sentence.
   ### Padding is the technique in which the number of words in a sentence is less than the limit set of words in a sentence then it is replaced by 0's.
   C. Feature representation is used while training the model for the dataset so that each word will be compared with every features for the better training of the dataset. Then we add the embedding layer with the help of embedding with dimensions in order to conver the text into vectors. Because we are creating the RNN model to do sentiment analysis of the review's so we used ReLU activation technique because ReLU allows positive values to pass through unchanged while setting all negative values to zero. We used Dense in creating RNN model because it has complete connections with the hidden layers and As the density of the connection increases, the number of paths through which the gradient flows is increased.

   D. Once we have code the layers of the model then we simply need to write model.build(input_shape, max_words ) so that all the layers can be presented as summary. Once done then in order to minimze the baises and weights we are going to set an optimizer as adam, loss as binary_crossentrophy and set metrics as accuracy to check the performance of the Model created.

   E. Because it is a large dataset so while training the model we will set an early stopping callback and maintain the patience of 5. Because we also have to deploy so one method is to save the file as 'file_name.h5' so that we can use the model to write the code for prediction.
5. Create a new Prediction file and get word_index of the dataset and create reverse_word_index. Then create functions to decode the review and pre-process the review so that any lower_case issue in the review can be resolved and does not affect the prediction of the review.
6. Once the prediction function is created then in order to create a UI for the users to input the review's and get the sentiment analysis of it, you can need to create a python file through which you can run on streamlit platform.

                                             
   






   

   


