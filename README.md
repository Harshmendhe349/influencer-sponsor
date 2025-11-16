# Influencer–Sponsor Platform

This is a full-stack Influencer Marketing and Sponsorship Management Platform built using Flask and SQLite. Sponsors can create campaigns, influencers can apply and negotiate, and admins can monitor all user and campaign activity.

---

## Features

### Sponsor Features
- Create and manage advertisement campaigns
- View incoming influencer ad requests
- Accept, reject, or negotiate with influencers
- Search influencers by category, niche, or reach
- Receive ML-based influencer recommendations

### Influencer Features
- Create and update public profile
- Browse active campaigns
- Send ad requests
- Negotiate with sponsors
- View request status (pending, accepted, rejected)

### Admin Features
- Full visibility into all users and campaigns
- View and manage flagged users and campaigns
- Monitor platform activity
- Root-level access to data

### ML Recommendation System
- Uses synthetic influencer dataset
- Includes preprocessing and training scripts
- Produces a trained model (.pkl)
- Suggests best-matched influencers for campaigns

---

## Tech Stack

Backend: Flask (Python)  
Frontend: HTML, CSS, Bootstrap, Jinja2  
Database: SQLite  
Machine Learning: Scikit-Learn, Pandas, NumPy  
Environment: Virtualenv or Pipenv  

---

## Project Structure

```
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
│── requirements.txt
│── .gitignore
│── README.md
```

---

## Installation

### 1. Clone the Repository
```
git clone https://github.com/Harshmendhe349/influencer-sponsor.git
cd influencer-sponsor
```

### 2. Create a Virtual Environment
```
python -m venv venv
venv\Scripts\activate        # Windows
# or
source venv/bin/activate    # Mac/Linux
```

### 3. Install Dependencies
```
pip install -r requirements.txt
```

### 4. Initialize Database
```
python create_db.py
```

### 5. Add Admin User
```
python add_admin.py
```

### 6. (Optional) Retrain Machine Learning Model
```
python preprocess_data.py
python train_model.py
```

### 7. Run the Application
```
python app.py
```

Application will run at:
```
http://127.0.0.1:5000/
```

---

## ML System Details

- `synthetic_influencer_data.csv` contains demo influencer dataset.
- `preprocess_data.py` prepares the dataset.
- `train_model.py` trains the recommendation ML model.
- `trained_model.pkl` stores the trained model.
- `recommendation_model.py` loads the model for predictions.

---

## Roadmap

- Add analytics dashboard
- Add payments / contract management
- Add JWT or OAuth authentication
- Add real influencer data import
- Add in-app chat for negotiations

---

## License
MIT License

---

## Author
Harsh Mendhe

