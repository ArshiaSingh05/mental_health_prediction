# 🧠 Mental Health Predictor – AI-Powered Web App

**Cognifit-AI** is an AI-based mental health prediction platform designed to assess an individual's mental wellness risk based on workplace-related and demographic factors. The system leverages a machine learning model trained on survey data to predict whether a person is at *high risk* or *low risk* of mental health issues.


## 🚀 Features

- 🔍 **User-Friendly Frontend**: Built using **React + Vite**, optimized for responsiveness and clean UI.
- 🔗 **FastAPI Backend**: Efficient REST API serving ML predictions with easy scalability.
- 📊 **ML Model**: Preprocessed and trained on a real mental health dataset.
- 🎯 **Risk Categorization**: Binary classification into `High Risk` or `Low Risk`.
- ⚙️ **Fully Integrated**: Frontend and backend combined into one deployable project.
- 🌐 **Auto Launch**: Web browser automatically opens the frontend upon backend startup.


## 🛠️ Tech Stack

| Component | Technology |
|----------|-------------|
| Frontend | React (Vite.js, HTML, CSS, JavaScript) |
| Backend | Python, FastAPI |
| ML Model | Scikit-learn |
| Deployment | Localhost (development) |
| Version Control | Git + GitHub |


## 📁 Project Structure

mental-health-predictor/
├── backend/
│ ├── api.py ← FastAPI app & prediction route
│ ├── model_utils.py ← Preprocessing logic & model loading
│ ├── mental_health_model.pkl← Trained ML model
├── cognifit-ai/
│ └── cognifit/
│ └── frontend/
│ ├── dist/ ← Production build of the frontend
│ ├── src/ ← React components & pages
│ └── index.html ← Main HTML file
└── README.md ← Project documentation


## 🧠 Machine Learning
- **Model Used**: Logistic Regression / Random Forest (customizable)
- **Input Features**: Includes 20+ attributes such as age, gender, workplace support, remote work, etc.
- **Target Output**: Binary (0 = Low Risk, 1 = High Risk)


## Backend Setup
cd backend
python -m venv venv
venv\Scripts\activate   # For Windows
pip install -r requirements.txt
uvicorn api:app --reload
## 🔁 Your browser will automatically launch at http://127.0.0.1:8000

## Frontend Setup (if modifying UI)
cd cognifit-ai/cognifit/frontend
npm install
npm run dev       # For development
npm run build     # For production

## 👥 Team Members

| Name | Contributions |
|----------|-------------|
| Arshia | Machine Learning model development, development and integration |
| Vansh | Complete frontend design, backend assistance |
| Surya | API design and integration, backend logic |
| Paras | Model deployment handling, FastAPI routing, error handling |

## 📌 Future Improvements
📲 Mobile app integration
☁️ Cloud deployment (Render/Heroku)
🧬 Deeper NLP-based mental health diagnosis
👨‍⚕️ Integration with therapy booking services
