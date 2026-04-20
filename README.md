# DeepDigit: Neural Network Digit Classifier

**DeepDigit** is an interactive deep learning application that identifies handwritten digits using a custom-trained Sequential Neural Network.

## 🧠 Model Architecture
* **Input Layer:** Flattens 28x28 pixel images into 784-dimensional vectors.
* **Hidden Layer:** 128 neurons with ReLU activation for feature extraction.
* **Output Layer:** 10 neurons with Softmax activation for digit probability ($0-9$).

## 🛠️ Tech Stack
* **Framework:** TensorFlow / Keras
* **UI:** Gradio (Interactive Sketchpad)
* **Processing:** NumPy, PIL (ImageOps)

## 🚀 Getting Started
1. **Install Dependencies:**
   ```bash
   pip install tensorflow gradio numpy pillow
