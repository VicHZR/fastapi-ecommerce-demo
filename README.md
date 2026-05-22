# 📦 FastAPI & Stripe Mini E-Commerce Backend

[![FastAPI](https://shields.io)](https://fastapi.tiangolo.com/)
[![Stripe](https://shields.io)](https://stripe.com/)
[![Docker](https://shields.io)](https://docker.com)
[![Python](https://shields.io)](https://python.org)

A production-ready asynchronously-powered asynchronous E-Commerce backend implementation using **FastAPI** integrated with **Stripe API** as the core transactional payment processor. This project focuses on high-performance endpoint delivery, dynamic content discovery via structured JSON processing, and containerized microservice deployment.

---

## 🎯 Key Technical Features

- **Asynchronous Payment Gateway:** Seamless integration with Stripe API infrastructure for secure, production-grade tokenized checkout transactions.
- **Dynamic File-Based Data Layer:** Automatic product discovery layer through server-side JSON schema parsing and dynamic directory indexing.
- **Containerized Architecture:** Fully dockerized ecosystem running isolated app containers orchestrated via **Docker Compose**.
- **Modern UI Styling:** Clean frontend implementation powered by the premium Soft UI Design System framework.

---

## 🏗️ Architectural Layout

The codebase is engineered to maintain low decoupling and structured execution flows under standard Python practices:

```text
fastapi-ecommerce-demo/
│
├── src/
│   ├── app.py             # Application entry point & API Router configuration
│   ├── static/            # Static assets management (product imagery)
│   └── templates/         # UI Components & JSON-driven product definitions
│
├── env.sample             # Environment variables template for Stripe API keys
├── Dockerfile             # Container blueprint definition
├── docker-compose.yml     # Multi-container orchestration specification
└── requirements.txt       # Production engine dependencies
```

---

## ⚙️ Installation & Local Setup

### 🐳 Option A: Quick Start via Docker (Recommended)

Ensure you have Docker and Docker Compose installed on your local host machinery, then run:

```bash
git clone https://github.com
cd fastapi-ecommerce-demo
docker-compose up --build
```
Once initialized, visit the container cluster hosting at `http://localhost:5085`.

### 💻 Option B: Manual Environment Build

#### 1. Setup Virtual Environment & Install Core Engines
```bash
virtualenv env
source env/bin/activate  # On Windows: env\Scripts\activate
pip install -r requirements.txt
```

#### 2. Configure Transactional Environment Variables
Rename the local blueprint `env.sample` to `.env` and fill in your secure sandbox credentials:
```env
STRIPE_SECRET_KEY=sk_test_...
STRIPE_PUBLISHABLE_KEY=pk_test_...
```

#### 3. Run the Backend Server
```bash
uvicorn src.app:app --reload
```
The local server will accept incoming traffic threads at `http://localhost:8000`.

---

## 🔌 API Testing & Live UI Documentation

FastAPI natively wraps the endpoint mappings into structured interactive UI platforms:

- **Swagger Interactive Testing Sandbox:** [http://localhost:8000/docs](http://localhost:8000/docs) – Ideal for manual or automated integration testing of backend operations.
- **ReDoc Architecture Layout:** [http://localhost:8000/redoc](http://localhost:8000/redoc) – Clean technical layout mapping schemas and response payloads.

---

## 🛡️ Financial Technical Practices Implemented

- **Secure Environment Tokenization:** Strict isolation of secure API payment keys from the application layer execution via environment mapping files (`.env`).
- **Dynamic Routing & Slugs:** Scalable URL mapping using algorithmic slug paths parsed directly out of JSON entities.
