# Fashion Recommendation System

This is an image-based fashion recommendation system built using ResNet50 and streamlit. 

## Overview

The system works by extracting image features from fashion images using a ResNet50 model pretrained on ImageNet. These image embeddings are stored and then used to find similar images based on Euclidean distance.

A streamlit frontend allows the user to upload a fashion image, extract its features, find the nearest neighbors in the dataset, and display the recommended similar fashion images.

## Goals

The goals of this project are:

- Provide an easy-to-use fashion recommendation system for users
- Allow users to find similar clothing items based on a image
- Learn how to build an image similarity engine using deep learning
- Gain experience deploying a web app with Streamlit and TensorFlow

## Data

The fashion images are stored in the `/images` folder. This can be extended by adding more fashion images of different types.

The image filenames and embeddings are pickled to `filenames.pkl` and `embeddings.pkl` respectively.

## Requirements

- TensorFlow 
- OpenCV
- Streamlit
- Numpy
- Pickle
- Sklearn
## Usage

The initial image embeddings are pre-generated and stored in `embeddings.pkl` using the `extract_features()` function. 

To run the streamlit app:

```
streamlit run app.py
```

This will launch the fashion recommendation web app. Upload an image and the app will display the top 5 recommended similar fashion images.

The recommend() function finds the nearest neighbors using sklearn's NearestNeighbors.

## Achievements
- Successfully built an image retrieval and recommendation engine 
- Extracted meaningful visual features from fashion images using a CNN
- Created an interactive web app using Streamlit
- Practiced deploying and serving a deep learning model
- Applied techniques like similarity search and image embeddings
## Future Work


- Use a larger dataset of fashion images for more variety
- Experiment with different CNN architectures for feature extraction
- Add image categories and filters to the app
- Deploy the app on a cloud service
## Contact

For any questions, feedback or suggestions, please reach me at gande.vi@northeastern.edu
