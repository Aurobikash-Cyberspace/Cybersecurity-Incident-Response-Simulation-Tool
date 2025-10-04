🛡️ Cybersecurity Incident Response Simulation Tool:

A full-stack simulation platform designed to replicate real-world cybersecurity incident response scenarios.
This tool helps analyze, detect, and respond to simulated cyber threats like phishing attacks, malware infections, and DoS attempts — all inside a controlled environment.

🚀 Features :

⚙️ FastAPI Backend: Efficient REST API built with Python and FastAPI.
🔐 Incident Simulation: Create and manage incident events dynamically.
🧠 Database Integration: SQLAlchemy-powered ORM for storing incidents.
💻 Frontend Dashboard: Interactive interface to visualize real-time incidents.
🌐 Cross-Platform Setup: Runs on Kali Linux (via UTM) with API access from the host browser.
🧩 Security Automation: Automates detection and response processes.

🧱 Project Structure :

incident-response-sim/
│
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── api_router.py
│   │   ├── api/
│   │   │   └── routes_incidents.py
│   │   ├── models/
│   │   │   └── incident.py
│   │   ├── schemas/
│   │   │   └── incident.py
│   │   └── core/
│   │       └── database.py
│   └── venv/
│
└── frontend/
    ├── index.html
    ├── app.js
    └── styles.css


⚙️ Installation & Setup:

*Backend Setup :

# 1️⃣ Navigate to the backend directory
cd backend

# 2️⃣ Activate virtual environment
source venv/bin/activate

# 3️⃣ Install dependencies
pip install fastapi uvicorn sqlalchemy

# 4️⃣ Run the FastAPI server
uvicorn app.main:app --host 0.0.0.0 --port 8000

*Frontend Setup :

# 1️⃣ Navigate to the frontend directory
cd frontend

# 2️⃣ Start a simple web server
python3 -m http.server 8080

🧪 Testing the API :

use Curl or Swagger UI :
curl http://127.0.0.1:8000/api/incidents/

🧰 Technologies Used :

Python 3
FastAPI
SQLAlchemy
Uvicorn
HTML, CSS, JavaScript
Kali Linux (via UTM)













