# Lstm_Lyrics_Gen

This notebook is a demonstration of using LSTM (Long Short-Term Memory) neural networks to generate lyrics. The model is trained on a dataset of lyrics and generates new lyrics based on the patterns it has learned.

## Getting Started

To run the notebook, you will need to have the following installed:
* Jupyter Notebook
* Python 3
* TensorFlow 2
* Keras
* Numpy
* Pandas
* Matplotlib

The notebook is divided into the following sections:
1. Data Preparation
2. Building the LSTM Model
3. Training the Model
4. Generating Lyrics

You can run the code by executing each cell in order.

## Data

The dataset used in this notebook is a collection of lyrics of songs scraped from the internet. The lyrics are preprocessed to remove special characters and lowercase all the letters.

## Results

The model is able to generate new lyrics that are coherent and similar to the lyrics in the training set. However, the generated lyrics are not always grammatically correct and might not make sense in certain contexts. That because the network was train to predict **using only one word at a time**.

## Conclusion

The LSTM_Lyrics_Gen notebook provides a glimpse into how LSTM neural networks can be used to generate creative text. Additionally, this notebook can be used as a starting point for experimenting with different architectures, hyperparameters, or datasets to improve the quality of the generated lyrics.

## Acknowledgements

This notebook is inspired by the work of [RomAmsili](https://github.com/RomAmsili) and the dataset used is from Ben Gurion University.


## The network Architecture :

![image](https://user-images.githubusercontent.com/82934994/213434902-4bd757e0-b7d7-48a4-9e93-1ce36b91091f.png)

## Training loss:

![image](https://user-images.githubusercontent.com/82934994/213435042-0bcd77b2-3b22-4303-a3b0-06fb7bee61ac.png)

## Sampling

Word generation was not deterministic. Using a softmax function on the probobilities from 'word_model.most_similar(positive=[np.array(pred)],topn=10)) the next word is  sampled.

![image](https://user-images.githubusercontent.com/82934994/213435427-71e00e25-af9d-4f08-a908-9f45bdc2a66e.png)

## Lyric example:

![image](https://user-images.githubusercontent.com/82934994/213435651-71e7dab4-7895-4669-a204-32bca2387d4a.png)

