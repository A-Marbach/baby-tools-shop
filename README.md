# Baby Tools Shop

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Docker Setup](#docker-setup)
- [Project Structure](#project-structure)
- [Links](#links)
- [Security Notes](#security-notes)

---

## Introduction
This repository contains the **Baby Tools Shop**, a Django-based e-commerce application for baby products.  
It includes a Docker setup for easy deployment and a structured project ready for local development or cloud deployment.

The purpose of this project is to showcase:

- Django development with models, views, and templates
- Dockerized deployment
- Secure handling of environment variables
- Complete project documentation

---

## Prerequisites
Before starting, make sure you have:

- Python 3.9+
- Django 5.x
- Docker & Docker Compose installed (optional)
- Git
- Access to a terminal

---

## Quick Start
### Clone the repository
```bash
git clone git@github.com:your-project.git
cd baby-tools-shop
git checkout future
Create a virtual environment 
bash
Code kopieren
python3 -m venv env
source env/bin/activate  # Linux/macOS
env\Scripts\activate     # Windows
Install dependencies
bash
Code kopieren
pip install -r requirements.txt
Run migrations and start the server
bash
Code kopieren
python manage.py migrate



Usage
Browse products by category

View product details

User registration and login

Filter products on the homepage

Add extra functionality 

Docker Setup
Build the Docker image
bash
Code kopieren
docker build -t babytools-shop .
Run the container



Notes
All migrations are applied automatically on container start.

ALLOWED_HOSTS must include the VM IP if running on a remote server.





Security Notes
Do not commit SSH keys, passwords, or API tokens to the repository.

Use environment variables for sensitive information.

Keep .env files outside version control.

Follow naming conventions: UPPER_CASE_WITH_UNDERSCORE for environment variables.

Reference variables using ${VAR_NAME} syntax in Dockerfiles or scripts.