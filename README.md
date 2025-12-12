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

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### Backend Setup

```bash
python server.py
```

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
