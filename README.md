# Insurance Premium Prediction API (FastAPI)

This project is a **FastAPI-based machine learning application** that predicts the **insurance premium** for a patient based on their personal and lifestyle information.

## 📌 Features
- Accepts user input through API requests:
  - Age
  - Weight
  - Height
  - Annual Income (LPA)
  - Smoker status
  - City
  - Occupation
- Predicts the estimated **insurance premium** using a trained machine learning model.
- Lightweight and fast API powered by **FastAPI**.
- JSON-based request and response format.

## 🚀 Tech Stack
- **Backend Framework:** FastAPI
- **Language:** Python
- **Machine Learning:** Scikit-learn / Joblib (for model loading)
- **Data Processing:** Pandas, NumPy
- **Server:** Uvicorn

## 📂 Project Structure
Insurance_premium_FastAPI/
│-- app.py # Main FastAPI application
│-- model.pkl # Trained ML model
│-- requirements.txt # Python dependencies
│-- README.md # Project documentation


## 🛠 Installation & Usage

1. **Clone the repository**
```bash
git clone https://github.com/<your-username>/Insurance_premium_FastAPI.git
cd Insurance_premium_FastAPI

Create a virtual environment and activate it
python -m venv env
# Windows
env\Scripts\activate
# Linux/Mac
source env/bin/activate

Install dependencies
pip install -r requirements.txt

Run the FastAPI server
uvicorn app:app --reload

Test the API
Open your browser and go to:
http://127.0.0.1:8000/docs

You can use the interactive Swagger UI to send requests.

📥 Example Request (JSON)
{
  "age": 35,
  "weight": 70,
  "height": 175,
  "income_lpa": 8,
  "smoker": "No",
  "city": "Pune",
  "occupation": "Engineer"
}
