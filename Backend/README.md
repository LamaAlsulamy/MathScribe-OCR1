# MathScribe-OCR – Backend

This directory contains the **backend implementation** of the MathScribe-OCR system.  
The backend is responsible for processing printed mathematical expression images and converting them into structured **LaTeX representations** using a deep learning–based OCR model.

The service is implemented using **FastAPI** and exposes a RESTful API that can be consumed by a web-based frontend.

---

## Backend Responsibilities

The backend performs the following tasks:

- Accepts image uploads containing printed mathematical expressions
- Processes images using a deep learning image-to-LaTeX model
- Reconstructs mathematical structure rather than plain text
- Returns LaTeX output along with performance metrics
- Logs inference results for evaluation and analysis

---

## Model Overview

The backend integrates **Pix2Tex**, a vision-to-sequence deep learning model designed specifically for **mathematical expression recognition**.

Unlike traditional OCR systems, the model:
- Understands spatial and hierarchical relationships
- Preserves fractions, superscripts, subscripts, and operator alignment
- Outputs valid LaTeX syntax representing the original expression

---

## Technologies Used

- **Python**
- **FastAPI** – Backend API framework
- **Uvicorn** – ASGI server
- **PyTorch** – Deep learning framework
- **Pix2Tex** – Image-to-LaTeX OCR model
- **Pillow (PIL)** – Image preprocessing
- **Requests** – Automatic model weight downloading

---

## How to Run the Backend

Follow the steps below to run the backend service locally:

### 1. Prerequisites
- Python 3.8 or higher
- pip package manager

### 2. Install Dependencies

Navigate to the backend directory and install the required packages then start the Server
run the FastAPI backend using the following command:

```bash
pip install -r requirements.txt
python server.py

