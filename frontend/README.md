# MathScribe-OCR – Frontend

This repository contains the **frontend interface** for the MathScribe-OCR system, a web-based application designed to support the recognition and transcription of **printed mathematical expressions** into LaTeX format.

The frontend provides an interactive user interface for uploading images, previewing recognized mathematical expressions, and exporting the generated LaTeX output.

---

## Project Overview

MathScribe-OCR is a full-stack system that integrates a deep learning–based backend for mathematical expression recognition with a modern web frontend for user interaction and visualization.

This frontend is responsible for:
- Accepting image inputs containing printed mathematical expressions
- Displaying rendered LaTeX output for validation
- Communicating with the backend inference API
- Supporting export and usability features for academic workflows

---

## Frontend Development Approach

The initial version of the frontend was **scaffolded using Lovable**, a rapid UI development platform, to accelerate interface design and component generation.

After the initial setup, the project was:
- Cloned and maintained locally
- Customized and extended using a standard React development workflow
- Integrated with a FastAPI-based backend via RESTful API calls

This hybrid approach allowed fast prototyping while preserving full control over the codebase.

---

## Technologies Used

The frontend is built using the following technologies:

- **React** – Component-based UI development
- **TypeScript** – Type-safe JavaScript
- **Vite** – Fast development server and build tool
- **Tailwind CSS** – Utility-first styling
- **shadcn/ui** – Reusable UI components

---

## Local Development Setup

To run the frontend locally:

```bash
# Navigate to the frontend directory
cd frontend

# Install dependencies
npm install

# Start the development server
npm run dev
