DeepDigit: Neural Network Digit Classifier

DeepDigit is an interactive deep learning application that identifies handwritten digits using a custom-trained Sequential Neural Network. Built with TensorFlow and Keras, this project demonstrates a complete AI lifecycle—from data normalization and model training to real-time inference via a web-based sketchpad.

🧠 Model Architecture

The model is trained on the classic MNIST dataset and utilizes a Feed-Forward Neural Network (FFNN) structure:

Input Layer: Flattens 28x28 pixel grayscale images into 784-dimensional arrays.

Hidden Layer: A dense layer of 128 neurons utilizing the ReLU (Rectified Linear Unit) activation function for non-linear feature extraction.

Output Layer: A dense layer of 10 neurons utilizing the Softmax activation function to output a probability distribution across the 10 possible digits (0-9).

🛠️ Tech Stack

Deep Learning Framework: TensorFlow / Keras

Web UI / Deployment: Gradio (Interactive Canvas/Sketchpad)

Image Processing: Pillow (PIL), NumPy, OpenCV

🚀 Getting Started

Prerequisites

Ensure you have Python installed, then install the required dependencies:

pip install tensorflow gradio numpy pillow matplotlib


Running the Application

Clone the repository and navigate to the project directory.

Run the Python script to train the model and launch the web interface:

python ai.py


Usage: Once the terminal provides a local URL (e.g., http://127.0.0.1:7860), open it in your browser. Draw any number between 0 and 9 on the provided sketchpad, and the model will display the top 3 most likely predictions in real-time.

⚙️ Data Pipeline & Preprocessing

To ensure high accuracy on user-drawn inputs, the Gradio interface automatically preprocesses the canvas data to match the MNIST training conditions:

Converts the RGBA canvas drawing to Grayscale ('L').

Inverts the colors (MNIST is trained on white digits over a black background).

Resizes the image to a standardized $28 \times 28$ pixel grid.

Normalizes pixel values from a $0-255$ scale to a $0.0-1.0$ scale.

📊 Training Results

The model is compiled using the Adam optimizer and Sparse Categorical Crossentropy loss. It consistently achieves >95% accuracy on the test dataset in just 2 training epochs, showcasing highly efficient gradient descent and pattern recognition.

📜 License

Distributed under the MIT License.
