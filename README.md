# Simple Items API (FastAPI + Docker)

## Overview

This is a minimal REST-style API built with FastAPI.

It exposes endpoints to manage items in memory:

- `GET /health` – health check
- `GET /items` – list all items
- `POST /items` – create a new item
- `GET /items/{item_id}` – get a single item by ID
- `DELETE /items/{item_id}` – delete a single item by ID

Data is stored in an in-memory list (no database), for learning purposes.

## Tech stack

- Python 3
- FastAPI
- Uvicorn
- Docker

## How to run locally (without Docker)

1. (Optional) Create and activate a virtual environment.

2. Install dependencies:
    pip install -r requirements.txt

3. Start the server:
    uvicorn main:app --reload

4. Install dependencies:
    pip install -r requirements.txt

5. Open:
    <http://127.0.0.1:8000>
    <http://127.0.0.1:8000/health>
    <http://127.0.0.1:8000/items>
    <http://127.0.0.1:8000/docs>
