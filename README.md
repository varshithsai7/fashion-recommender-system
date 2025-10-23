# fashion-recommender-system
A Deep Learning based Fashion Recommender System using the ResNET50
📖 Overview

This project presents a Deep Learning-based Fashion Recommendation System that suggests similar fashion items based on visual features. Using ResNet50, a pre-trained Convolutional Neural Network, the system learns deep visual patterns from fashion images and recommends visually similar clothing items.

It’s an AI-powered approach to modern fashion — combining the art of aesthetics with the science of machine intelligence.

🎯 Objective

The goal of this project is to build a content-based recommendation system that can:

Identify visual similarities between outfits

Recommend items with comparable style, color, and texture

Provide a personalized fashion browsing experience

🧠 Model Architecture

This system leverages ResNet50, a deep residual network pre-trained on ImageNet.

Transfer Learning: Utilized ResNet50 to extract feature embeddings from fashion images.

Feature Extraction: Removed the top layer and extracted 2048-dimensional embeddings.

Similarity Matching: Used cosine similarity / Euclidean distance to recommend the top-N similar items.

📂 Dataset

Dataset used: Fashion Product Images (Small)

~44,000 images of fashion products

Attributes include category, gender, article type, base color, and more

Each image represents a single fashion product

⚙️ Technologies Used

Python 3.10+

TensorFlow / Keras

NumPy, Pandas

Matplotlib / Seaborn

scikit-learn

ResNet50 (pre-trained model)

🚀 Workflow

Data Preprocessing:

Cleaned and resized images to 224x224

Removed missing and invalid entries

Feature Extraction:

Loaded ResNet50 without the top layer

Converted each image into a fixed-length feature vector

Similarity Computation:

Computed pairwise cosine similarities

Recommended top 5 most visually similar products

Interface (optional extension):

Integrated a simple Flask / Streamlit UI for image input and recommendations display
