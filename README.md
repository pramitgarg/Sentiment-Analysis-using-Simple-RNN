# Sentiment-Analysis-using-Simple-RNN
This project shows the simple RNN used to do text classification of movie review's given by IMDB and using streamlit to display and then deploy it on Streamlit Cloud. 

In this Project, we have download the datasets from the tensorflow and build the RNN model. Here are the steps taken to execute this project : 
1. Creating the Gituhb repo and clone the repo on VS code on my local system.
   
2. Creating an virtual environment with [ python -m venv .venv ] and activate the environment by source  activate/bin/.venv. Downloading libraries like ipykernel, tensorlfow, keras etc in the requirements.txt file and installing all the libraries through pip install -r requirements.txt.

3. Created Embedding.ipynb file and converted a sample text into embeddings. The steps involved in converting text into embeddings are :                                     
   A. First, we are going to set the vocabulary words so that there is a limited word from the dataset which is converted and on which model is trained so that the model can be more effecient and fast.                                                                                                                                              
   B. Using one_hot technique which converts the words [ categorical variables ] into Vectors [ binary format]                                                           
   C. We import libraries like Embedding, Pad_sequence, sequential where Pad_sequence fills the 0 to pre or post in the line where the words are less than the limit set for each line. 
   D. Feature prepresentation dimenstion are going to be set so that each word can be compared with the dimensions set.                                                            
   e. Using Sequential model technique in order to create RNN model because Sequential processing ensures that instructions are executed in a predictable and ordered manner, allowing for reliable and consistent results.     

3. Creating RNN Model in SimpleRNN.ipynb file
   

   


