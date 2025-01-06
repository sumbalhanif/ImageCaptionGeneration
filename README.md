# ImageCaptionGeneration
Preprocessing:
I used the Flickr dataset, which contains both images and captions. First, I cleaned the dataset, created a vocabulary, and then used a tokenizer. I mapped the captions to the images and saved them in a dictionary where the image name is the key, and the caption is the value. These are the preprocessing steps.
Model:
After that, I used a CNN-RNN (Encoder-Decoder) model. For CNN, I used InceptionV3 to extract image features, and for RNN, I used LSTM (Long Short-Term Memory) to process caption sequences. Additionally, for word embeddings, I used GloVe (Global Vectors), which is an unsupervised learning algorithm that provides pre-trained word embeddings files that are easily available. I also used a decoder that concatenates the images with the captions to generate the output.
After setting up the layers of the model, I trained it for 50 epochs and used greedy search to generate predictions from the model. You can see the model's predictions in the pictures below. 😊
