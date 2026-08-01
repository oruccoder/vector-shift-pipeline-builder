# 🚀 VectorShift Pipeline Builder

A full-stack, visual workflow pipeline builder inspired by VectorShift. Built with **React Flow** on the frontend and **FastAPI** on the backend. It features custom node abstractions, dynamic variable parsing, auto-resizing text components, and DAG (Directed Acyclic Graph) cycle detection algorithms.

---

## ✨ Features

- **Node Abstraction (`BaseNode`)**: Reusable base component to rapidly create styled nodes with dynamic handles and layout without repeating UI code.
- **Dynamic Handle Generation**: Automatically extracts variables enclosed in double curly brackets (e.g., `{{ input }}`) from the Text node and renders corresponding target handles.
- **Auto-Resizing UI**: Textarea within nodes dynamically adjusts its height based on user input.
- **DAG Validation (Cycle Detection)**: Backend service uses **Kahn's Algorithm (BFS Topological Sort)** to analyze pipeline edges and detect invalid loops.
- **Custom Nodes Included**:
  - `Input` & `Output` Nodes
  - `LLM` Node
  - `Text` Node (with variable extraction)
  - `Filter` Node
  - `Select` Node
  - `API Request` Node
  - `Note` Node
  - `Math Operation` Node

---

## 🛠️ Tech Stack

- **Frontend**: React.js, React Flow, Zustand (State Management)
- **Backend**: Python, FastAPI, Pydantic, Uvicorn

---

## 🚀 Getting Started

### 1. Prerequisites
- Node.js (v16 or higher)
- Python 3.8+

---

### 2. Setup Frontend

```bash
cd frontend
npm install
npm start
