Image-Based Recommendation System (DIO Project)
-Project Overview

This project implements a visual recommendation system that suggests similar products based only on image appearance (shape, texture, and visual patterns), rather than textual metadata such as brand, price, or model.

The system compares a query image (teste.jpg) with a dataset of product images and recommends the most visually similar items using OpenCV and ORB descriptors.


-Objective

Build a simple content-based image recommendation system capable of retrieving visually similar products from an image database.


- Technologies Used

Python

OpenCV (ORB + BFMatcher)

NumPy


- How to Run
Folder structure: (Create a folder in Drive called seu_projeto with the following structure)

seu_project/

│── recomendar.py (code)

│── teste.jpg

└── dataset/ (Create a folder with several images of silver necklaces, rings, and earrings.)
    ├── img1.jpg
    ├── img2.jpg
    └── ...
Steps:

Install dependencies:

pip install opencv-python numpy

Place your query image as teste.jpg.

Add product images inside the dataset/ folder.

Run:

python recomendar.py

Two windows will appear:

Query Image

Top 5 Visual Recommendations


- How It Works

Extracts visual features using ORB.

Compares features with all dataset images.

Ranks images by visual similarity.

Displays the most similar products on screen.

Save embeddings to speed up search

Use KNN for faster retrieval

Add product categories (e.g., shoes, watches, shirts)

Build a web or graphical interface
