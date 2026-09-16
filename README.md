# deep-learning-fashion-classification
# Deep Learning Fashion Image Classification

A beginner-friendly Deep Learning project using **TensorFlow/Keras** to classify fashion product images into 10 different categories.

## 📌 Project Overview

This project demonstrates how an Artificial Neural Network can be used to automatically classify product images.

The project uses the **Fashion MNIST** dataset, which contains grayscale images of common fashion products.

### Business Scenario

Imagine an e-commerce company receiving thousands of product images every day.

Instead of manually categorizing every image, a Deep Learning model can predict the appropriate product category automatically.

**Input:** Product image
**Output:** Predicted product category

## 🎯 Objectives

* Understand how images can be used as Deep Learning inputs.
* Build a simple Artificial Neural Network.
* Understand input, hidden and output layers.
* Train a model using labelled image data.
* Evaluate model accuracy on unseen data.
* Use the trained model to classify new images.
* Connect an AI model to a real-world business problem.

## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Jupyter Notebook
* Fashion MNIST Dataset

## 👕 Product Categories

The model classifies images into 10 categories:

1. T-shirt/Top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle Boot

## 🧠 Model Architecture

The project uses a simple Artificial Neural Network:

```text
28 × 28 Image
      ↓
Flatten
      ↓
Dense Layer — 64 neurons
      ↓
ReLU Activation
      ↓
Dense Layer — 10 neurons
      ↓
Softmax
      ↓
Predicted Category
```

### Key Components

* **Flatten:** Converts the 28×28 image into a format that can be processed by the neural network.
* **Dense(64):** Hidden layer that learns patterns from the image.
* **ReLU:** Activation function used in the hidden layer.
* **Dense(10):** Produces an output for each of the 10 product categories.
* **Softmax:** Converts the outputs into category probabilities.

## 🔄 Project Workflow

```text
Fashion MNIST Dataset
        ↓
Data Loading
        ↓
Image Visualization
        ↓
Data Normalization
        ↓
Neural Network Creation
        ↓
Model Training
        ↓
Model Evaluation
        ↓
Prediction
        ↓
Business Interpretation
```

## 📊 Data Preparation

The original image pixels have values between **0 and 255**.

They are normalized to values between **0 and 1**:

```python
train_images = train_images / 255.0
test_images = test_images / 255.0
```

This makes the image data easier for the neural network to process.

## 🏋️ Model Training

The model is trained using:

* Optimizer: `Adam`
* Loss function: `Sparse Categorical Crossentropy`
* Metric: `Accuracy`
* Epochs: `3`
* Validation split: `10%`

## 📈 Model Evaluation

After training, the model is evaluated using test images that were not used during training.

The project calculates:

```text
Test Accuracy
```

Accuracy represents the proportion of test images that the model classified correctly.

## 💼 Business Application

An e-commerce company could use a similar system to assist with product categorization.

### Traditional Process

```text
Product Image
     ↓
Employee manually identifies category
     ↓
Product listed
```

### AI-Assisted Process

```text
Product Image
     ↓
Deep Learning Model
     ↓
Predicted Category
     ↓
Human Review (if required)
     ↓
Product Listed
```

### Potential Benefits

* Faster product listing
* Reduced repetitive manual work
* More consistent categorization
* Improved product search and organization
* Ability to process large numbers of images

## ⚠️ Limitations

The model will not classify every image correctly.

Before deploying a similar system in a real business, factors such as:

* Incorrect classifications
* Training-data quality
* Customer experience
* Cost of errors
* Human review

should be considered.

## 📁 Project Structure

```text
deep-learning-fashion-classification/
│
├── Deep_Learning_Fashion_Classification_Name.ipynb
└── README.md
```

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Install dependencies

```bash
pip install tensorflow matplotlib numpy
```

### 3. Open the notebook

Open:

```text
Deep_Learning_Fashion_Classification_Name.ipynb
```

using Jupyter Notebook or VS Code.

### 4. Run the cells

The Fashion MNIST dataset will be downloaded automatically when the notebook is executed.

## 📚 Learning Outcomes

This project demonstrates the basic workflow of an image-classification Deep Learning model:

**Data → Preprocessing → Neural Network → Training → Testing → Prediction → Business Application**

---

## 👨‍💻 Author

**Anshit**

BBA (FinTech & AI) Student

Interested in Finance, Artificial Intelligence, Data Analytics and Quantitative Finance.
