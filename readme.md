# Beginner Command Reference

This README contains commonly used beginner commands for **Conda**, **Docker**, **Flask**, **Git**, **Linux**, plus **Docker Compose** and **Conda export/import**.

---

## 📌 1. Conda Commands

Check Conda version:
conda --version

Create a new environment:
conda create --name myenv python=3.11

Activate environment:
conda activate myenv

Deactivate environment:
conda deactivate

List all environments:
conda env list

Install packages:
conda install numpy pandas

Remove an environment:
conda remove --name myenv --all

Export environment to YAML:
conda env export > environment.yml

Create environment from YAML:
conda env create -f environment.yml

---

## 📌 2. Docker Commands

Check Docker version:
docker --version

Pull an image:
docker pull imagename

Build image from Dockerfile:
docker build -t imagename .

Run a container (map port 5000):
docker run -d -p 5000:5000 imagename

List running containers:
docker ps

Stop a container:
docker stop container_id

Remove a container:
docker rm container_id

Remove an image:
docker rmi imagename

View Docker logs:
docker logs container_id

---

## 📌 3. Docker Compose Commands

Start services:
docker-compose up

Start services in detached mode:
docker-compose up -d

Stop services:
docker-compose down

Rebuild services:
docker-compose up --build

---

## 📌 4. Flask Quick Start

Install Flask:
pip install flask

Create `app.py`:
from flask import Flask
app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, Flask!"

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000, debug=True)

Run Flask app:
python app.py

Access the app:
http://127.0.0.1:5000

---

## 📌 5. Git Basics

What is Git?
Git is a version control system used to track code changes and collaborate.

Configure Git:
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

Initialize a repository:
git init

Clone a repository:
git clone https://github.com/user/repo.git

Check status:
git status

Add changes:
git add .

Commit changes:
git commit -m "Your commit message"

Push to remote:
git push origin main

Pull latest changes:
git pull origin main

Show branches:
git branch

Switch branch:
git checkout branch_name

Create branch:
git branch new_branch

Merge branch:
git merge branch_name

View commit history:
git log

---

## 📌 6. Basic Linux Commands

ls             # List files
cd folder      # Change directory
pwd            # Show current directory
mkdir dir      # Create directory
rm file        # Remove file
rm -r dir      # Remove directory
touch file.txt # Create empty file
cat file.txt   # View file contents

---

## ✅ Quick Workflow Summary

1. **Conda:**  
conda create --name myenv python=3.11  
conda activate myenv  

2. **Docker:**  
docker build -t app .  
docker run -d -p 5000:5000 app  

3. **Flask:**  
Create app.py → python app.py  

4. **Git:**  
git init → git add . → git commit -m "msg" → git push  

---


