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
## Frontend Setup

This section explains how to run the frontend interface of the **MathScribe-OCR** project locally.

The frontend is a web-based user interface that allows users to upload images of mathematical expressions and view the LaTeX output returned by the backend.

---

### Prerequisites

Before running the frontend, make sure the following tools are installed on your machine:

* **Node.js (LTS version recommended)**
  Node.js is required to run the JavaScript development server.
  The project was tested using **Node.js v20 (LTS)**.

* **npm (Node Package Manager)**
  npm is used to install project dependencies and run scripts.
  It is included automatically when installing Node.js.

You can verify installation by running:

```bash
node -v
npm -v
```

---

### Run the Frontend Locally

Follow these steps to start the frontend application:

1. Navigate to the frontend directory:

```bash
cd frontend
```

2. Install all required dependencies:

```bash
npm install
```

This command downloads and installs all JavaScript libraries needed by the frontend (such as React, Vite, and UI components).

3. Start the development server:

```bash
npm run dev
```

4. Open your browser and go to:

```
http://localhost:8080
```

The frontend interface should now be running and ready to use.

---

### Notes

* The frontend runs on a local development server using **Vite**.
* Make sure the **backend server is running** in parallel so the frontend can send image requests and receive LaTeX results.
* If any dependency errors occur, deleting `node_modules` and running `npm install` again usually resolves the issue.

