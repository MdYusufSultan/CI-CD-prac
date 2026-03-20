Create Project Folder
mkdir ml-cicd-project
cd ml-cicd-project
-----------------------
python -m venv venv
venv\Scripts\activate
pip install pandas scikit-learn pytest joblib
=========================
Create ML Training Script
Create Test Case
Create folder:mkdir tests
tests/test_model.py
--------------------------------------
Run Locally
python train.py
pytest
--------------------------------
Create GitHub Repository

Go to GitHub

Click New Repository

Name: ml-cicd-project

Click Create   
================================
Push Code to GitHub

git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/your-username/ml-cicd-project.git
git push -u origin main
==================================
Create GitHub Actions Workflow
Create folders: mkdir -p .github/workflows

Create file: .github/workflows/ci.yml
=================================
Push Workflow

git add .
git commit -m "Added CI pipeline"
git push
===================================
View Pipeline Execution

Go to GitHub repo

Click Actions tab

You will see pipeline running
======================git add .
git commit -m "Update training"
git push