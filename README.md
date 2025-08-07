# heroku-flask-ci-cd
My first Python Flask app with CI/CD pipeline and Heroku deployment
# Flask CI/CD Demo App (Heroku Ready)

This is a sample Python Flask application built for learning cloud deployment and CI/CD pipelines.  
It is designed to be deployed on **Heroku** with full automation and testing in place.

# Tech Stack

- Python 3.10
- Flask (web framework)
- Gunicorn (production WSGI server)
- GitHub Actions (CI/CD)
- Pytest (unit testing)
- Bandit (security scanning)
- Heroku (platform for deployment)

# Features

- Clean project structure with modular code
- CI/CD pipeline:
  - Runs on each `push` or `pull request`
  - Executes unit tests
  - Scans for security issues (e.g., `debug=True`)
- Heroku-ready with `Procfile`, `runtime.txt`, and buildpack support
- Logging and monitoring (planned after deployment)

# Local Setup

git clone https://github.com/balajirasamsetti/heroku-flask-ci-cd.git
cd heroku-flask-ci-cd
python -m venv venv
venv\Scripts\activate    # (or source venv/bin/activate on Mac/Linux)
pip install -r requirements.txt
python app/app.py

# Run Tests

pytest

# Run Security Scan

bandit -r app

# Deployment to Heroku (Waiting for account verification)

heroku login

heroku create your-app-name

git push heroku main

heroku open

