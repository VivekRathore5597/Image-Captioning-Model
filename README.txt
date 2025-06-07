 Image Captioning Model using Deep Learning
============================================

This project demonstrates an end-to-end image captioning system using deep learning. It leverages the Flickr8K dataset and combines CNN-based image feature extraction with an LSTM-based caption generator.

Dataset
- Flickr8K Dataset
- Contains 8,000 images with 5 human-annotated captions per image.
- Source: https://www.kaggle.com/datasets/adityajn105/flickr8k

Note: The dataset must be downloaded manually from Kaggle due to terms of service.

 Model Architecture
1. Feature Extraction:
   - Pretrained CNN model (Xception) used to extract image embeddings.
   - Extracted features saved as `.keras` files (e.g., feature_extractor.keras).

2. Caption Generation:
   - Tokenizer converts text captions to sequences.
   - A custom neural network with Embedding + LSTM layers is used to generate captions from image features.
   - Final model saved as model.keras.

 Dependencies
---------------
- TensorFlow / Keras
- NumPy
- PIL (Pillow)
- tqdm

 Results
The model generates simple but meaningful captions such as:
    Input: A dog running through a field
    Output: "a dog is running in the grass"

 Notes
- The Flickr8K dataset must be preprocessed before training.
- Training on the full dataset may take several hours on a GPU.
- You can use Google Colab or Kaggle notebooks for training.

Acknowledgements
- Kaggle – Flickr8K Dataset: https://www.kaggle.com/datasets/adityajn105/flickr8k
- Deep Learning Specialization by Andrew Ng
