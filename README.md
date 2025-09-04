# AI-Handwriting-Digit-Recognizer
A web application that recognizes handwritten digits (0–9) using a deep learning model trained on the MNIST dataset. Users can draw a digit on the canvas, and the AI predicts the number in real time with confidence scores. Built with Vue.js, Node.js, and TensorFlow.


# 🖊️ Handwriting Digit Recognizer
A simple AI-powered web application that can recognize handwritten digits (0–9).  
The user draws a digit on the canvas, and the trained deep learning model predicts the number in real time.  

## Features
- Draw digits directly in the browser (canvas)
- Automatic preprocessing (28x28 grayscale normalization)
- AI model trained on the **MNIST dataset**
- Displays predicted digit with **confidence score**
- Built with **Vue.js (frontend)** + **Node.js/Python backend** + **TensorFlow**

---

## How It Works
1. User draws a digit (0–9) on the canvas.  
2. The image is converted into a **28x28 grayscale matrix**.  
3. Values are normalized from **0–255 → 0–1**.  
4. The data is passed into a **Convolutional Neural Network (CNN)** trained on the MNIST dataset.  
5. The model returns a prediction with probabilities for each digit.  

---
## AI Model Architecture (CNN – Convolutional Neural Network)
We use a **CNN** because it’s the most effective type of model for image recognition.

### Typical CNN layers for MNIST:
1. **Input Layer**
    - Shape: (28x28x1) → the normalized image.
2. **Convolutional Layers**
    - Detect basic patterns (edges, lines, curves).
    - Example: 32 filters of size 3x3.
3. **Pooling Layers**
    - Reduce image size while keeping important features.
    - Example: MaxPooling (2x2).
4. **Flatten Layer**
    - Converts the 2D feature maps into a 1D vector.
5. **Dense (Fully Connected) Layers**
    - Classic neural network layers that combine the extracted features.
    - Usually with **ReLU activation**.
6. **Output Layer**
    - 10 neurons (one for each digit: 0–9).
    - Uses **Softmax activation** → returns probabilities that sum to 1.
---
##  Tech Stack
- **Frontend:** Vue.js, HTML5 Canvas, CSS3  
- **Backend:** Node.js (Express) or Python Flask  
- **AI Model:** TensorFlow / Keras (MNIST dataset)  
- **Other Tools:** GitHub, VS Code, Docker (optional)  

---

## Installation & Setup

### Clone the repo
    ```bash
    git clone https://github.com/Yosefnademo/handwriting-digit-recognizer.git
c   d handwriting-digit-recognizer


### Install dependencies
    npm install   # for frontend/backend
    pip install -r requirements.txt   # if using Python backend

### Run the app
    npm run dev    # start frontend
    npm run server # start backend (or python app.py)


## 📸 Demo




## 📜 License

This project is licensed under the MIT License – see the [LICENSE](/LICENSE)
 file for details.

