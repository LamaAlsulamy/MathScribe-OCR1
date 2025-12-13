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

## Backend Setup

### Prerequisites

* Python 3.9 or higher
* pip
* (Optional but recommended) Conda or virtual environment

---

### 1. Navigate to Backend Directory

First, move to the backend folder:

```bash
cd backend
```

---

### 2. Install Dependencies

Install all required Python packages listed in the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

---

### 3. Run the Backend Server

Start the FastAPI backend server using:

```bash
python server.py
```

Once the server is running, the backend API will be available locally and ready to receive requests from the frontend.

---

## ⚠️ Recommended Setup (Conda / Compatibility Fix)

Some deep learning libraries used in this project are **not fully compatible with NumPy 2.x**.
To avoid runtime errors, we strongly recommend downgrading NumPy before installing dependencies.

### Step 1: Remove Current NumPy Version

```bash
pip uninstall numpy -y
```

### Step 2: Install a Compatible NumPy Version

```bash
pip install "numpy<2"
```

### Step 3: Reinstall Project Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the Backend Server

```bash
python server.py
```

---

### 🧠 Notes

* The backend is built using **FastAPI** for high-performance inference.
* It handles image uploads, runs the OCR model, and returns LaTeX predictions.
* Make sure the backend is running **before** starting the frontend.
