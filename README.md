# 📦 FastAPI & Stripe Mini E-Commerce Backend

<p align="left">
  <a href="https://fastapi.tiangolo.com/">
    <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  </a>
  <a href="https://stripe.com/">
    <img src="https://img.shields.io/badge/Stripe-635BFF?style=for-the-badge&logo=stripe&logoColor=white"/>
  </a>
  <a href="https://docker.com">
    <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  </a>
  <a href="https://python.org">
    <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  </a>
</p>

---

## 🚀 Overview

A **production-ready asynchronous E-Commerce backend** built with **FastAPI**, integrated with **Stripe API** for secure, tokenized payment processing infrastructure. 

This project demonstrates:
- ⚡ High-performance asynchronous API design leveraging non-blocking execution pools.
- 💳 Secure payment integration workflows following fintech tokenization standards.
- 🐳 Enterprise containerized deployment orchestration.
- 📦 Dynamic file-based data modeling and schema management.

🎯 Focus: **Scalability, asynchronous concurrency processing, and fintech-grade backend architecture.**

---

## 🎯 Key Technical Features

- ⚡ **Asynchronous Payment Gateway**  
  Native implementation of Stripe API infrastructure inside asynchronous event-driven endpoints to maximize concurrent transaction request handling.

- 📂 **Dynamic File-Based Data Layer**  
  Product catalog and business assets driven entirely through automatic server-side JSON schema parsing and dynamic system directory indexing.

- 🐳 **Containerized Architecture**  
  Fully containerized production ecosystem utilizing structured **Dockerfiles** and orchestrated multi-container configurations via **Docker Compose**.

- 🎨 **Frontend Integration**  
  Clean, high-fidelity responsive user interface decoupled and powered by the premium Soft UI Design System framework.

---

## 📊 Impact (CV-Level Highlights)

- 🚀 **High Concurrent Request Capacity:** Achieved efficient request routing throughput under heavy thread loads using Python's native asynchronous architecture (`asyncio`).
- 💳 **Fintech-Grade Data Isolation:** Mitigated PCI-compliance security risks by implementing full Stripe checkout tokenization, ensuring zero sensitive cardholder data footprint on the server.
- 🐳 **Consistent Dev-to-Prod Environment:** Eliminated local hosting alignment bugs by engineering a completely reproducible architecture through Docker software environments.
- 📈 **Optimized Response Latency:** Drastically slashed processing thread execution times across order placement and transactional validation endpoints through async-driven I/O non-blocking operations.

---

## 🏗️ Project Structure

```text
fastapi-ecommerce-demo/
│
├── src/
│   ├── app.py             # FastAPI entry point, application router, and endpoint controllers
│   ├── static/            # Static assets management (product imagery and media resources)
│   └── templates/         # UI View components and JSON-driven structural product entities
│
├── env.sample             # Decoupled environment variables blueprint configuration
├── Dockerfile             # Container orchestration and layer configuration blueprint
├── docker-compose.yml     # Multi-container multi-thread microservice orchestration
└── requirements.txt       # Production execution dependency Manifest
```

---

## ⚙️ Installation & Setup

### 🐳 Option A: Docker Deployment (Recommended)

Ensure you have Docker and Docker Compose set up on your machine, then execute:

```bash
git clone https://github.com
cd fastapi-ecommerce-demo
docker-compose up --build
```

📍 The container network will listen to API traffic hosting at:
- **Local Application Hub:** [http://localhost:5085](http://localhost:5085)

---

### 💻 Option B: Manual Infrastructure Setup

#### 1. Initialize Virtual Environment
```bash
virtualenv env
source env/bin/activate  # On Windows use: env\Scripts\activate
```

#### 2. Install Project Engine Dependencies
```bash
pip install -r requirements.txt
```

#### 3. Configure Secure Environment Variables
Rename the local layout blueprint `env.sample` to `.env` and fill in your private payment gateway keys:
```env
STRIPE_SECRET_KEY=sk_test_...
STRIPE_PUBLISHABLE_KEY=pk_test_...
```

#### 4. Run the Uvicorn Application Engine
```bash
uvicorn src.app:app --reload
```

📍 Local server threads will accept connection requests at:
- **Local Server Engine:** [http://localhost:8000](http://localhost:8000)

---

## 🔌 API Documentation & Live Inspection

FastAPI automatically parses routing metadata and maps it into interactive runtime API engines:

- 📘 **Swagger UI Sandbox:** [http://localhost:8000/docs](http://localhost:8000/docs) – Ideal for execution testing and automated functional integration validations.
- 📗 **ReDoc Architectural Mapping:** [http://localhost:8000/redoc](http://localhost:8000/redoc) – Specialized technical structure for payload schema structural analysis.

---

## 🔐 Security Practices

- **Zero-Footprint Tokenization:** Integration relies strictly on secure client-side payment tokens, preventing local database exposure to unauthorized data extraction.
- **Strict Environment Separation:** Critical credentials and keys are isolated using independent environment parsing files (`.env`), avoiding sensitive data leaks in version control repositories.
- **Decoupled API Routing Infrastructure:** Backend logic handles webhook transaction checks independently from the frontend layer to avoid client-side injection attempts.
- **Server-Side Payload Validation:** Input requests are dynamically filtered against structural Pydantic validation parameters before execution.

---

## 🧠 Tech Stack

- **Backend Architecture:** FastAPI (Python 3.11+)
- **Payment Processing Core:** Stripe Developer Tools API
- **Infrastructure Virtualization:** Docker & Docker Compose
- **Front-End Styling Framework:** HTML5 + CSS3 + Soft UI Engine
- **Structural Paradigm:** Asynchronous, Cloud-Ready, Microservice Architecture

---

## 🔥 Future Improvements

- [ ] Implement secure stateful session handling via JWT (JSON Web Tokens) Authentication.
- [ ] Migrate data layer management into a relational engine database such as PostgreSQL via SQLAlchemy ORM.
- [ ] Incorporate comprehensive historical order tracking structures.
- [ ] Engineer continuous integration and deployment pipelines using GitHub Actions workflows.

---

## 👨‍💻 Author

**Victor Guzmán**  
*Computational Scientist | Backend Engineer | Software Quality & Test Automation Specialist*  
- 🔗 **LinkedIn:** [https://linkedin.com](https://www.linkedin.com/in/victor-h-guzm%C3%A1n-a19361187/)
