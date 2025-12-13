# MathScribe-OCR

**A Printed Mathematical Expression Recognition and LaTeX Conversion System**

## 1. Introduction

MathScribe-OCR is a full-stack system designed for the recognition and structural transcription of **printed mathematical expressions**. The system converts symbols and typeset mathematical formulas into LaTeX markup through an integrated visual recognition engine and user-facing interface. The goal of this work is to support educational digitization, formula indexing, and mathematical content restructuring in academic and computational environments.

## 2. Research Problem

Printed mathematical notation represents spatial, symbolic, and hierarchical structures that cannot be interpreted through basic OCR character-level extraction. Mathematical expressions involve superscripts, fractions, integrals, matrices, and positional alignment that require symbolic reconstruction rather than plain text detection. The system addresses the need for accurate and structured printed formula transcription.

## 3. System Objectives

* To detect printed mathematical symbols and their spatial relationships.
* To reconstruct mathematical expressions into standardized LaTeX format.
* To provide an interactive interface for verification, display, and export.

## 4. System Components

### 4.1 Frontend Interface (React + Vite + Tailwind)

* Visual display of uploaded mathematical expressions.
* LaTeX rendering preview for validation.
* Export options and interactive output handling.

### 4.2 Backend Processing Layer

* Symbol recognition and structural parsing engine.
* Conversion of printed notations into LaTeX representation.
* API-based communication with the frontend for real-time inference.

### 4.3 Output Layer

* Generation of LaTeX code.
* Rendered visual output to ensure layout accuracy and alignment consistency.
## 5. Implementation Requirements

This project consists of two main parts:

* **Frontend** (React + Vite)
* **Backend** (FastAPI + OCR Model)

Both parts must be running for the system to work correctly.

---

## Frontend Setup

### Prerequisites

* **Node.js (LTS version – v20.x recommended)**
* npm (comes with Node.js)

> Important:
> Using very new Node.js versions may cause dependency issues with Vite.
> We recommend using **Node.js v20 (LTS)**.

---

### 1. Navigate to Frontend Directory

```bash
cd frontend
```

---

### 2. Install Dependencies

```bash
npm install
```

This command installs all required frontend libraries listed in `package.json`.

---

### 3. Run the Frontend Development Server

```bash
npm run dev
```

After running the command, the frontend will be available at:

```
http://localhost:8080
```

---

## Backend Setup

### Prerequisites

* **Python 3.9 or higher**
* pip
* (Optional but recommended) Conda or virtual environment

---

### 1. Navigate to Backend Directory

```bash
cd backend
```

---

### 2. Install Dependencies

Install all required Python packages:

```bash
pip install -r requirements.txt
```

---

### 3. Run the Backend Server

```bash
python server.py
```

Once running, the FastAPI backend will start locally and listen for requests from the frontend.

---

## Recommended Setup (NumPy Compatibility Fix)

Some deep learning libraries used in this project are **not compatible with NumPy 2.x**.
To avoid runtime errors, follow these steps **before installing dependencies**:

### Step 1: Remove Current NumPy Version

```bash
pip uninstall numpy -y
```

### Step 2: Install a Compatible Version

```bash
pip install "numpy<2"
```

### Step 3: Reinstall Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the Backend

```bash
python server.py
```

---

### Notes

* The **backend must be running first** before using the frontend.
* The backend performs OCR inference and returns LaTeX results.
* The frontend provides the user interface for image upload and result visualization.
## 6. Workflow Summary

1. User provides printed mathematical expression input.
2. Backend processes the notation and extracts symbolic structure.
3. Expression is reconstructed into LaTeX.
4. Frontend displays the resulting transcription with export capability.

## 7. Evaluation Summary

Preliminary evaluation indicates stable performance in printed symbol detection and accurate LaTeX transcription. Fractional forms, superscripts, and operator alignment demonstrate consistency across multiple samples.

## 8. Conclusion

MathScribe-OCR serves as a digitization and transcription tool for printed mathematical content. It enables accurate structural reconstruction and supports academic formula archiving, instructional content development, and publication workflows.

## 9. Scholarly Contribution

* Enhances accessibility of printed mathematical content in digital environments.
* Supports LaTeX-oriented academic publishing standards.
* Provides structured transcription verification for educational and research contexts.

## Model Reference

The backend of MathScribe-OCR is built upon the Pix2Tex (Image-to-LaTeX) model, which is an open-source vision-to-sequence deep learning architecture designed for mathematical expression recognition.

The model implementation is based on the following repository:

https://github.com/lukas-blecher/LaTeX-OCR

This repository provides the core image-to-LaTeX transcription pipeline that enables structural reconstruction of printed mathematical expressions.


## 10. Team Information

**Project Contributors**

| Name                      |
| ------------------------- |
| Maram Moshabbab Al Romman |
| Lama Muidh Alsulami       |
| Rimas Yasir Allehaibi     |
| Layan Munwer Almoqati     |
| Lama Mousa Alzahrani      |
