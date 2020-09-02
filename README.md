# Sentiment-Analysis
This repo consists of Sentiment Analysis and EDA on Movie Reviews by NLTK Data.

[NOTEBOOK](https://nbviewer.jupyter.org/github/guljain/Sentiment-Analysis/blob/master/Notebook.ipynb)

![image](https://drive.google.com/uc?export=view&id=1JWoF3K_X2PRwAGFbMceiRW5KdH5CSIc0)
![image](https://drive.google.com/uc?export=view&id=1ZzsoK1JgeWiWTkO2i4XU00pX7bhczSc3)
![image](https://drive.google.com/uc?export=view&id=1JawnQvWzju2ggPw7wrG3D1idwcdkfmSt)


# Data 
Link to data is [Here](https://drive.google.com/drive/folders/1w2INX9wxHJ-jtEN2UcKUni4Qri3xqzJS?usp=sharing)

Structure :

- Sentiment analyis
  - Movie Reviews
    - Neg
    - Pos
    - Side Stuff


# Motivation 
NLP has always been a challenging topic in machine learning. The best use of NLP is in detecting what the majority wishes for and hence, SENTIMENT ANALYSIS.

# Work Done
1. Cleaned the data
2. Performed EDA 
3. Created encodings (self, using frequency and Bert Encodings)
4. Implemented :
      - Ranfom Forest Regressor
      - Logistic Regression
      - Neural Network 
      - Encoding Model

# EDA
Various plots like word cloud, pie, donut, histograms etc were used for performing EDA on the dataset. Top common words from negative sentiment and positive sentiment were displayed in form of donut, bars. For common words, pie chart was additionally made. Various plots of words cloud were included in the begining of the notebook. Plots of the validation and training loss are also displayed. 

# Models
Various models were implemented :
1. Logistic Regression - Using Bert Embedding, it gave 50 % accuracy
2. Random Forest Regressor - Using Bert Embedding, it gave 40-45 % accuracy
3. EMbedding models - Using encoding made of top 1000 words and series of length of 350, the accuracy achieved was 50 %
4. Bert Encoding - Using Bert Encoding and class model with various Dense layers and embedding and glove method, 79-80 % accuracy was achieved

# Key Work
Tried to generate polarities and build plots to show the distribution of negative and positive sentiments. It used top 500 negative words and 500 positve words such that any word is not present in both of the encoding.

# Key Observation
A drastic reduction in the frequency of words was observed when the threshold was set to 5.

# Further Improvements that can be made
1. Sarcasm detection was not taken in account.
2. The Bert encoding was padded to maximum length and thus lots of 0s were there for Logistic Regression and Random Forest methos, making the apporpiate padding can help achieve better base models.
3. SVM and many other methods can be combined to give a better accuracy.

# Some links
WORD ClOUD - https://towardsdatascience.com/create-word-cloud-into-any-shape-you-want-using-python-d0b88834bc32
Make WORD CLOUD with different fonts - https://www.dafont.com 
