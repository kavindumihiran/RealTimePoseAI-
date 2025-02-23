# RealTimePoseAI-
This contains a simple real-time pose recognition system using Mediapipe for landmark detection and a custom-made CNN-LSTM sequential model for classification.This model dtects three poses,
* Both hands up
* Left hand up
* Hands crossed

# Technologies Used 🛠️
* Programming Language: Python,
* Frameworks & Libraries:,
  * TensorFlow/Keras,
  * OpenCV (cv2),
  * Mediapipe ,
  * NumPy, Pandas,

# Features 📌
1. Real time pose detection
   * Uses Mediapipe to ecxtract the facial and body landmarks.
   * Captures real-time video feed and detect these poses.
   * Processes images frame-by-frame for live pose recognition.

2. Custom datase creation
   * Collected 100 images per pose using OpenCV (cv2) in jupyter Notebook.
   * Dataset includes three pose classe:
      * Both hands up
      * Left hand up
      * Hands crossed

3. CNN-LSTM Model for pose classification
   * 5-layer architecture:
     * **First 3 layers:** LSTM layers to capture temporal patterns.
     * **Final 2 layers:** Dense layers for classification.
   * Activation Functions:
     * **ReLU** for hidden layers.
     * Softmax for output layer (multi-class classification)
   * Optimizer: Adam for efficient convergence.
   * Training:
     * **1500 epochs** for accutare model learning.
     * Achieved 100% accuracy on the three-class dataset.

4. Live Pose Prediction
   * Takes live input from a webcam.
   * Extract body landmarks using Mediapipe.
   * Passes landmark coordinates to the trained CNN-LSTM model.
   * Outputs real-time pose classification results.

# How to Run the Project 🚀
* pose_recognition.ipynb contais the code for the project,
* pose_recognitio_model.h5 is the trained model with 100 images for each class.
* You can run this in either jupyter notebook, Google colab or any similar environment.
* 1️⃣ Install Dependencies
```bash
pip install tensorflow opencv-python mediapipe numpy pandas
```
* 2️⃣ Run the Jupyter Notebook
```bash
jupyter notebook
```
* 3️⃣ Train the Model (if needed)
* 4️⃣ Run Real-Time Pose Detection

# Future Improvements 📌
* Expand the dataset with more poses and more data for each class
* Implement gesture-based control for smart applications.
* Improve model generalization to different lighting and camera angles 
