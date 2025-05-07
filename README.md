#  Skin Cancer Classifier (Deep Learning Project)

This is our mini project where we built a web app to classify skin cancer images using deep learning.  
We used the **HAM10000** dataset and trained a CNN model, and then used **Flask** for the backend and **React** for the frontend.

---

##  What it does

- You can upload a skin image (like a mole or lesion)
- Our model will predict what type of skin issue it might be (like melanoma, nevus, etc.)
- Shows the result on the website along with the confidence level

---

##  Tech Used

- **Deep Learning** (CNN with Keras/TensorFlow)
- **Python** for backend (Flask)
- **React JS** for frontend
- Dataset: [HAM10000](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000)

---

## Folder Structure

skin-cancer-classifier/
│
├── backend/ # Flask server + DL model
│ ├── app.py
│ ├── model/ # Saved model file (.h5)
│ └── requirements.txt
│
├── frontend/ # React UI
│ └── src/
│
└── README.md



---

## How to Run It

### Backend

```bash
cd backend
python -m venv venv
venv\Scripts\activate  # For Windows
pip install -r requirements.txt
python app.py
The backend will start at: http://localhost:5000

Frontend
bash
Copy code
cd frontend
npm install
npm start
The frontend will open at: http://localhost:3000

Model Training (Short Info)
We trained a CNN using Keras on the HAM10000 dataset.
We resized the images, normalized them, used some data augmentation, and trained for several epochs.
After training, we saved the model (.h5) and used it in our Flask backend to make predictions.

Notes
This is just for learning purposes and not for real medical use

We didn’t use a database — it's a simple frontend-backend setup

Model prediction might not be 100% accurate



