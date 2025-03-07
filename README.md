# Fashion MNIST Classification with Keras

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-brightgreen)

A neural network model to classify Fashion MNIST images using TensorFlow/Keras.
---

## Overview
This project trains a deep learning model to classify fashion items (e.g., shirts, shoes) from the Fashion MNIST dataset. The model achieves **~88% validation accuracy** and **~87% test accuracy**.
---

## Key Features
- **Data Visualization**: Sample images and training curves.
- **Model Architecture**: Fully connected neural network with one hidden layer.
- **Training**: 10 epochs, batch size of 64, Adam optimizer.
- **Evaluation**: Test accuracy and prediction visualization.
---

## Dataset
The **Fashion MNIST dataset** contains 70,000 grayscale images (28x28 pixels) across 10 categories:
- T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot.

**Source**: [Fashion MNIST on GitHub](https://github.com/zalandoresearch/fashion-mnist)
---

## Model Architecture
```python
model = Sequential([
    Flatten(input_shape=(28, 28)),
    Dense(128, activation='relu'),
    Dense(10, activation='softmax')
])
```

- Loss Function: ```sparse_categorical_crossentropy```
- Optimizer: Adam
- Metrics: Accuracy
---

## Results
### Training Progress
![image](https://github.com/user-attachments/assets/39d89e5f-8db9-4a26-9d67-2d3a3a90398a)

*Training vs validation accuracy/loss over epochs.*

### Sample Predictions
![image](https://github.com/user-attachments/assets/f710238b-5554-4050-b4aa-c1feda05005f)

*Green = correct prediction, Red = incorrect prediction.*

**Final Test Accuracy:** 87.3%

---

## GitHub Repository Structure
```
Fashion-MNIST-Classification/
├── notebooks/                 # Jupyter notebooks
│   └── Fashion_MNIST.ipynb   # Main notebook with code and visualizations
├── README.md                 # Project documentation
└── requirements.txt          # Dependencies
```
---

## Installation  
1. Clone the repository:
```
git clone https://github.com/zain-ul-abideen-5036/Fashion-MNIST-Classification.git
cd Fashion-MNIST-Classification
```
2. Install dependencies:
```
pip install -r requirements.txt
```
---

## Usage
1. Run the Jupyter notebook:
```
jupyter notebook notebooks/Fashion_MNIST.ipynb
```
2. Execute all cells to:
    - Load and visualize data.
    - Train the model.
    - Generate plots.
---

## Contact
For questions or feedback, contact: abideen5036@gmail.com
---
