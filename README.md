# 🚦 Smart Traffic Prediction & Congestion Management System

The **Smart Traffic Prediction & Congestion Management System** is a full-stack, intelligent application designed to monitor, analyze, and forecast traffic patterns in real-time. It integrates a high-performance Python FastAPI backend—powered by machine learning models—with a modern Next.js and Tailwind CSS web dashboard providing comprehensive multi-view traffic management capabilities.

---

## 🚀 Tech Stack

### **Frontend**

* **Framework:** Next.js (React / TypeScript)
* **Styling:** Tailwind CSS
* **UI Components & Icons:** Custom modular dashboard components, Lucide Icons, and Victory charts.

### **Backend**

* **Framework:** FastAPI (Python)
* **Server:** Uvicorn
* **Data Processing & ML:** Scikit-learn, Pandas, NumPy, Joblib (Random Forest models, feature/label encoders)

---

## 📂 Project Structure

```text
smart-traffic-prediction-congestion-management-system/
├── backend/
│   ├── app/                 # FastAPI application routes, schemas, and core logic
│   ├── data/                # Dataset files and data generation scripts
│   ├── venv/                # Python virtual environment
│   ├── requirements.txt     # Python dependencies
│   ├── train_model.py       # ML model training script
│   ├── prepare_ml_dataset.py# Dataset preparation scripts
│   ├── traffic_rf_model.pkl # Trained Random Forest traffic model
│   ├── feature_encoders.pkl # Feature encoding artifacts
│   └── label_encoder.pkl    # Label encoding artifacts
│
├── frontend/
│   ├── public/              # Static assets, icons, and svgs
│   ├── src/
│   │   ├── app/             # Next.js App Router (pages, login, layouts, globals)
│   │   │   └── components/  # Modular views & training manual assets
│   │   └── ...
│   ├── package.json         # Node.js dependencies
│   └── tsconfig.json        # TypeScript configuration
│
└── .gitignore               # Excludes node_modules, venv, .next, and build artifacts

```

---

## ✨ Core Features & Functional Views

* **Live Traffic Monitoring Dashboard (`TrafficMonitoringView` & `DashboardView`):** Real-time monitoring of city junctions, road utilization metrics, vehicle counts, and average speeds.
* **Interactive Live Map (`LiveMapView`):** Visual geographical layout tracking live congestion points and vehicle telemetry.
* **AI Forecasting Engine (`ForecastingView`):** Integrated machine learning pipeline utilizing trained Random Forest regressors to predict future vehicle density and congestion levels.
* **Analytics & Reports (`AnalyticsView` & `ReportsView`):** Comprehensive deep-dives into historical traffic data, trend graphs, performance metrics, and downloadable reporting tools.
* **Road Management (`RoadManagementView`):** Administrative tools for managing road networks, speed limits, and signal states.
* **User Authentication & Profile (`ProfileView` & Login):** Secure user sessions, authentication state management, and personalized user profiles.
* **Training Resources Integration:** Embedded technical manuals (e.g., PLC Training Manual) directly accessible within the system interface.

---

## ⚙️ Getting Started & Local Setup

### **1. Backend Setup**

Open a terminal, navigate to the backend directory, activate your virtual environment, and start the API server:

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000

```

### **2. Frontend Setup**

Open a separate terminal window, navigate to the frontend directory, install dependencies, and start the development server:

```bash
cd frontend
npm install
npm run dev

```

Open [http://localhost:3000](http://localhost:3000) in your web browser to access the dashboard interface.
