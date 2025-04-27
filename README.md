Web Nethralaya is an AI-driven, full-stack web platform designed to assist healthcare professionals in the early detection of Glaucoma and Retinopathy of Prematurity (ROP) through rapid, reliable analysis of eye fundus images.

Built with a lightweight HTML/CSS/JavaScript frontend and a robust Flask backend, the system leverages a custom-trained Convolutional Neural Network (CNN) developed using PyTorch to perform real-time predictions.
Users can upload retinal images via a simple web interface and instantly receive diagnostic feedback powered by deep learning.

This platform was designed with a focus on speed, accuracy, and accessibility, making it suitable for clinical environments, screening camps, and research studies aiming to reduce preventable vision loss.

Key Features
Custom-trained AI Model: CNN model (ResNet50-based) fine-tuned on fundus image datasets for Glaucoma and ROP detection.

Fast Frontend: Lightweight, responsive HTML5/CSS3/JavaScript frontend for a seamless experience.

Flask Backend: Python Flask server hosting the trained PyTorch model for inference.

Privacy Focus: No data storage. Images are processed in-memory and deleted post-inference.

Training Pipeline Included: Full Jupyter Notebook provided showing model building, training, evaluation, and visualization.

Tech Stack
Frontend: HTML5, CSS3, JavaScript

Backend: Python, Flask, PyTorch

Libraries: Torchvision, Pillow, NumPy

Project Structure
pgsql
Copy
Edit
WebNethralaya/
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── backend/
│   ├── app.py
│   ├── model.pth
│   └── requirements.txt
├── notebook/
│   └── G_L.ipynb
├── images/
│   ├── before_preprocessing.png
│   ├── after_preprocessing.png
│   └── heatmap.png
└── README.md
Sample Images from Model Pipeline

Original Image	After Preprocessing	GradCAM Heatmap
How to Run Locally
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/WebNethralaya.git
Install backend dependencies:

bash
Copy
Edit
pip install -r backend/requirements.txt
Start the Flask server:

bash
Copy
Edit
cd backend
python app.py
Open frontend/index.html in your browser.

Upload a fundus image ➔ Get real-time AI predictions!

📚 Notebook and Model Training
The full model training process, including:

Dataset preprocessing

Model fine-tuning

Evaluation metrics (accuracy, F1 score)

GradCAM visualization experiments
are available in the G_L.ipynb notebook!

Feel free to explore, reproduce, and retrain!