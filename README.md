📣 Influencer–Sponsor Platform

A full-stack Influencer Marketing & Sponsorship Management Platform built using Flask, SQLite, and Machine Learning.
Sponsors can create campaigns, influencers can apply and negotiate, and admins can monitor all activity in one unified system.

🚀 Features
⭐ Sponsor Dashboard

Create and manage advertising campaigns

View influencer ad requests

Accept, reject, or negotiate

Search influencers by category/niche

Get ML-based influencer recommendations

⭐ Influencer Dashboard

Create and update public profile

Browse active campaigns

Send ad requests

Negotiate with sponsors

Track request status (pending/accepted/rejected)

⭐ Admin Dashboard

Monitor all users and campaigns

View flagged influencers/sponsors

Flag campaign violations

Full system oversight

⭐ AI Recommendation System

Uses synthetic influencer dataset

Preprocessing and training scripts included

Generates a .pkl ML model

Recommends best influencers for campaigns

🧠 Tech Stack

Backend: Flask (Python)
Frontend: HTML, CSS, Bootstrap, Jinja2
Database: SQLite
ML: Pandas, NumPy, Scikit-Learn
Environment: Virtualenv / Pipenv

📁 Project Structure
influencer-sponsor/
│── app.py
│── create_db.py
│── add_admin.py
│── synthetic_influencer_data.csv
│── preprocess_data.py
│── train_model.py
│── recommendation_model.py
│── trained_model.pkl
│── templates/
│── static/
│── migrations/
│── Pipfile
│── Pipfile.lock
│── .gitignore
│── README.md

⚙️ Installation
1️⃣ Clone Repository
git clone https://github.com/Harshmendhe349/influencer-sponsor.git
cd influencer-sponsor

2️⃣ Create Virtual Environment
python -m venv venv
venv\Scripts\activate      # Windows
# OR
source venv/bin/activate  # Mac/Linux

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Initialize Database
python create_db.py

5️⃣ Add Admin User
python add_admin.py

6️⃣ (Optional) Train ML Model
python preprocess_data.py
python train_model.py

7️⃣ Run the Server
python app.py


Open in browser:

http://127.0.0.1:5000/

📦 ML System Overview

synthetic_influencer_data.csv: sample influencer dataset

preprocess_data.py: cleans & encodes dataset

train_model.py: trains model and saves trained_model.pkl

recommendation_model.py: loads model and predicts recommendations

🧭 Roadmap

Advanced analytics dashboard

Payment/contract workflow

Real influencer data integration

JWT-based authentication

Chat system for negotiation

📜 License

MIT License

👤 Author

Harsh Mendhe

If this project helped you, please ⭐ star the repository!
