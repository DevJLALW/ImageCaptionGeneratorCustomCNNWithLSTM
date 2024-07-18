### ImageCaptionGeneratorCustomCNNWithLSTM

Created a custom model for image captioning, training the model, extracting image features, and generating captions for both your dataset images and some external images. Here’s a step-by-step summary:
Step-by-Step Summary:

## Downloading Datasets:
flickr8k: https://www.kaggle.com/datasets/adityajn105/flickr8k
stl10: https://www.kaggle.com/datasets/jessicali9530/stl10

## Extracting Datasets:
Extracted datasets to specific directories.

## Model Creation and Compilation:
Created a custom CNN model for feature extraction.
Compiled the model with Adam optimizer and SparseCategoricalCrossentropy loss.

## Training the Model:
Loaded the STL-10 dataset.
Preprocessed images.
Trained the model with Early Stopping and Learning Rate Reduction callbacks.

## Feature Extraction:
Extracted features using the custom model.
Saved extracted features in a pickle file.

## Caption Processing:
Loaded captions and created mappings.
Cleaned captions and tokenized text.

## Model for Image Captioning:
Created an encoder-decoder model using LSTM and CNN features.
Trained the model with image-caption pairs.

## Caption Generation:
Generated captions for test images.
Calculated BLEU scores.

## Download and Generate Captions for External Images:
Downloaded images from URLs.
Extracted features for these images.
Generated captions for downloaded images.
