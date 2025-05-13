# 🖼️ Image Similarity Search for Movie Posters

This project demonstrates how to build an **image similarity engine** that finds visually similar movie posters using deep learning. The system leverages a pretrained CNN model to extract embeddings from movie posters, and retrieves similar images using nearest-neighbor search.

## 🚀 Features

- Downloads movie poster images using TMDb API.
- Extracts visual features using a pretrained deep learning model (e.g., ResNet50 or VGG).
- Computes image similarity using cosine or Euclidean distance.
- Visualizes the most similar posters to a given query.

## 📁 Project Structure

```text
ImageSimilaritySearch.ipynb # Main notebook with the full pipeline
posters/ # Folder where poster images are stored
```


## 🛠️ Requirements

Install the necessary dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow keras requests Pillow
```
You’ll also need an API key from TMDb to download movie posters.

## 🔧 How It Works

Poster Download: Use TMDb API to fetch poster images for a list of movie IDs.
Feature Extraction: Load a pretrained CNN and extract embeddings from each image.
Similarity Search: Compute pairwise distances and retrieve the top-N most similar images.
Visualization: Display the query image and its most visually similar posters.
## 📸 Example Output

Example:

Query Poster: Thor
Top 5 similar posters: Ironman, Armageddom, The Fifth Element, etc.

![Screenshot 2025-05-13 at 20 46 16](https://github.com/user-attachments/assets/1bec4768-8efc-40a7-9668-a0694cecc6e2)


## 📌 Notes

Some movie IDs may return 404 errors if posters are not available on TMDb.
The similarity search is based on visual features only, not metadata like genre or actors.
## 🙌 Acknowledgments

The Movie Database (TMDb)
Keras Applications for pretrained models
