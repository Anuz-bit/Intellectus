# Intellectus — Student Risk Analysis System 📊🎓

[![Frontend](https://img.shields.io/badge/Frontend-React%20%2B%20Vite-blue)](#tech-stack)
[![Backend](https://img.shields.io/badge/Backend-FastAPI-success)](#tech-stack)
[![ML](https://img.shields.io/badge/ML-scikit--learn-orange)](#tech-stack)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen)](#)
[![Live Demo](https://img.shields.io/badge/Demo-GitHub%20Pages-black)](https://anuz-bit.github.io/Intellectus/)

A hackathon-ready prototype for **early student risk detection** that combines spreadsheet data, rule-based analytics, and explainable machine learning to help institutions identify **at-risk students** and enable timely interventions.  
Frontend is deployed on GitHub Pages; the FastAPI + ML backend runs locally. :contentReference[oaicite:1]{index=1}

---

## 🌐 UI Preview (GitHub Pages)

🔗 https://anuz-bit.github.io/Intellectus/

> **Heads-up:** This is a **frontend-only preview**.  
> The **FastAPI + ML backend runs locally** (see **Run Locally** section).

---

## ✨ Features

- Upload multiple student datasets
- Machine Learning-based risk prediction
- Fast, scalable backend using FastAPI
- Modern, responsive UI
- Simple and clean interface
- Easy to run locally :contentReference[oaicite:4]{index=4}

---

## 🧱 Tech Stack

**Frontend**
- React (Vite)
- Tailwind CSS
- JavaScript :contentReference[oaicite:5]{index=5}

**Backend**
- Python
- FastAPI :contentReference[oaicite:6]{index=6}

**Machine Learning**
- Pandas, NumPy
- scikit-learn
- Joblib :contentReference[oaicite:7]{index=7}

---

## 📁 Project Structure

```text
Intellectus/
├── asset/                         # Screenshots used in README
├── backend/
│   ├── main.py                    # FastAPI backend & ML logic
│   ├── train_model.py             # Model training script
│   ├── student_risk_model.joblib  # Trained ML model
│   ├── feature_names.joblib
│   ├── fee_status_encoder.joblib
│   └── venv/                      # Local virtual environment (do not commit)
└── frontend/
    ├── src/                       # React source code
    ├── public/
    └── package.json
````

---

## ✅ Prerequisites

* Python **3.9+**
* Node.js **18+**
* npm

Verify installations:

```bash
python --version
node --version
npm --version
```

---

## 🚀 Run Locally (Step-by-Step)

### 1) Clone the repository

```bash
git clone https://github.com/Anuz-bit/Intellectus.git
cd Intellectus
```

---

### 2) Backend (FastAPI + ML)

```bash
cd backend
python -m venv venv
```

Activate the virtual environment:

**Windows**

```bash
venv\Scripts\activate
```

**macOS/Linux**

```bash
source venv/bin/activate
```

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

> If `requirements.txt` is missing, install manually:

```bash
python -m pip install pandas numpy scikit-learn joblib fastapi uvicorn python-multipart openpyxl
```

Start the backend server:

```bash
uvicorn main:app --reload
```

Backend runs at:

* [http://127.0.0.1:8000](http://127.0.0.1:8000)

API docs (if enabled):

* [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

### 3) Frontend (React + Vite)

Open a **new terminal**:

```bash
cd frontend
npm install
npm run dev
```

Frontend runs at:

* [http://localhost:5173](http://localhost:5173)

---

## 🧪 Usage

1. Open the app: `http://localhost:5173`
2. Upload the datasets:

   * `students.xlsx`
   * `academic_records.csv`
   * `activity_records.csv`
3. Click **Analyze Data**
4. Review results in:

   * Risk distribution dashboard
   * Student risk overview table
   * Individual student detail view ([GitHub][1])

> Tip: If you provide sample datasets in the repo later, link them here (e.g., `data/` folder) to make onboarding faster.

---

## 🖼️ Screenshots

| Home / Upload           | Dashboard                         |
| ----------------------- | --------------------------------- |
| ![Home](asset/home.png) | ![Dashboard](asset/dashboard.png) |

| Risk Table                          | Student Detail                              |
| ----------------------------------- | ------------------------------------------- |
| ![Risk Table](asset/risk_table.png) | ![Student Detail](asset/student_detail.png) |

---

## 🛣️ Roadmap

Planned improvements:

* Interactive dashboards
* Authentication (Admin / Teacher)
* Database integration
* Automated alerts
* Cloud deployment ([GitHub][1])

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a feature branch:

   ```bash
   git checkout -b feat/your-feature
   ```
3. Commit your changes:

   ```bash
   git commit -m "Add: your feature"
   ```
4. Push the branch:

   ```bash
   git push origin feat/your-feature
   ```
5. Open a Pull Request

### Development guidelines

* Keep PRs focused and small
* Update docs when behavior changes
* Prefer readable code + clear naming
* Add minimal validation for uploaded files (schema/columns) where applicable
---

## 👨‍💻 Author

**Anuj Wankhede**
B.Tech Student | Machine Learning & Data Analytics Enthusiast

[1]: https://github.com/Anuz-bit/Intellectus "GitHub - Anuz-bit/Intellectus: A hackathon-ready prototype for early student risk detection that combines spreadsheet data, rule-based analytics, and explainable machine learning to prevent dropouts through timely intervention and low-cost implementation."
