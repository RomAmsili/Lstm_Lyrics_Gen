# Lstm_Lyrics_Gen
Lyrics Generation using LSTM
Train a neural net to generate lyrics based on the provided melody.

During the training of the model I used both to the lyrics of a song and its melody.

The melodies are stored in .mid (MIDI files) and contain various types of information – notes, the instruments used etc. 

## The network Architecture :

![image](https://user-images.githubusercontent.com/82934994/213434902-4bd757e0-b7d7-48a4-9e93-1ce36b91091f.png)

## Training loss:

![image](https://user-images.githubusercontent.com/82934994/213435042-0bcd77b2-3b22-4303-a3b0-06fb7bee61ac.png)

## Sampling

Word generation was not deterministic. Using a softmax function on the probobilities from 'word_model.most_similar(positive=[np.array(pred)],topn=10)) the next word is  sampled.

![image](https://user-images.githubusercontent.com/82934994/213435427-71e00e25-af9d-4f08-a908-9f45bdc2a66e.png)

## Lyric example:

![image](https://user-images.githubusercontent.com/82934994/213435651-71e7dab4-7895-4669-a204-32bca2387d4a.png)

