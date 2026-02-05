# 🖋️ Digit Recognizer: CNN with TensorFlow & Gradio

This project implements a **Deep Learning** solution for the [Kaggle Digit Recognizer Competition](https://www.kaggle.com/competitions/digit-recognizer). It uses a **Convolutional Neural Network (CNN)** to classify handwritten digits (0-9) from the MNIST-style dataset with high accuracy.

## 🚀 Project Overview

The goal is to take a  pixel grayscale image of a handwritten digit and correctly identify the number. This repository covers the entire pipeline:

* **Data Acquisition:** Using `kagglehub` for direct API downloads.
* **Preprocessing:** Reshaping and Normalizing pixel values.
* **Architecture:** A multi-layer CNN built with Keras/TensorFlow.
* **Deployment:** An interactive UI using Gradio to visualize the dataset.

---

## 🛠️ Tech Stack

* **Language:** Python
* **Deep Learning:** TensorFlow / Keras
* **Data Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Interface:** Gradio

---

## 🧬 Model Architecture

The model uses a sequential approach designed to extract spatial features from the images:

1. **Convolutional Layer (32 filters, 3x3):** Detects basic edges and textures.
2. **MaxPooling (2x2):** Reduces spatial dimensions.
3. **Convolutional Layer (64 filters, 3x3):** Detects more complex shapes.
4. **MaxPooling (2x2):** Further downsampling.
5. **Convolutional Layer (64 filters, 3x3):** High-level feature extraction.
6. **Flattening:** Converts 3D feature maps to a 1D vector.
7. **Dense Layer (128 units):** Fully connected layer for classification logic.
8. **Output Layer (10 units):** Softmax activation to return probabilities for digits 0-9.

---

## 📊 Performance

* **Normalization:** Pixels scaled from  to .
* **Optimizer:** Adam
* **Loss Function:** Categorical Crossentropy
* **Validation Split:** 30% of the training data.

---

## 💻 How to Run

1. **Clone the repo:**
```bash
git clone https://github.com/your-username/digit-recognizer-cnn.git

```


2. **Install Dependencies:**
```bash
pip install tensorflow pandas numpy matplotlib seaborn kagglehub gradio colorama

```


3. **Authenticate Kaggle:**
Make sure you have your `kaggle.json` credentials set up to download the data via `kagglehub`.
4. **Execute the Notebook:**
Run the cells to train the model and launch the Gradio interface.

---

## 🌟 Interactive Demo

The project includes a **Gradio** interface. Users can input a digit (0-9), and the script will fetch a corresponding handwritten sample from the MNIST dataset to show how the data looks to the model.

---

## 📜 License

This project is open-source and available under the MIT License.

