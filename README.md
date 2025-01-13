# Image Gallery Web App

A web application that allows users to search and save images from Unsplash. The app uses a React frontend and a Flask backend, with MongoDB for storing user-saved images.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Backend Setup](#backend-setup)
- [Frontend Setup](#frontend-setup)
- [Deployment](#deployment)
- [Challenges & Improvements](#challenges-improvements)

## Project Overview

This web app provides a platform to search for random images from Unsplash and store them in a personal collection. Users can search for images by keywords, view images, and save their favorite ones for later use.

### Key Features:
- Search for random images based on a query (via Unsplash API)
- Save selected images to a MongoDB database
- View saved images in a gallery
- Delete saved images

## Technologies Used

- **Frontend**: React, Axios (for API calls), React Hooks
- **Backend**: Flask, MongoDB (via `pymongo`)
- **Deployment**: Docker, Docker Compose, AWS EC2 (optional)
- **Environment Management**: Python `pipenv`, React `npm`

## Installation

### 1. Clone the repository
```bash
git clone https://github.com/Vaishnav88sk/image-gallery.git
cd image-gallery
```

### 2. Setup the Backend (Flask)
```bash
cd backend
pip install -r requirements.txt
```
Or, using pipenv:
```bash
pipenv install
```
Setup .env.local:
```bash
UNSPLASH_KEY=your_unsplash_api_key
DEBUG=True
```
Run the Flask App:
```bash
python main.py
```

### 3. Setup the Frontend (React)
```bash
cd frontend
npm install
```
Run the React App:
```bash
npm start
```

### 4. Running the Full App with Docker Compose
```bash
docker-compose up --build
```
