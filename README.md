# 🍬 Candy Magic App

**Candy Magic App** is a full-stack web application designed for both desktop and mobile devices. It integrates a deep learning model to offer intelligent features, such as price prediction, and displays real-time product pricing to clients.

This monorepo contains the following components:

- 🔮 `frontend/` — User interface built with React or Next.js
- 🧠 `fastapi-service/` — Python backend using FastAPI for ML/DL predictions
- 🧾 `node-service/` — Node.js backend for user management and pricing API

## 📦 Project Structure

```
Candy-Magic-App/
│
├── frontend/             # Frontend app (React or Next.js)
├── fastapi-service/      # FastAPI backend for ML model
├── node-service/         # Node.js backend for pricing/auth
├── docker-compose.yml    # Optional: orchestrates all services
└── README.md             # Project documentation
```

## 🚀 Getting Started

### Step 1: Clone the repository

```bash
git clone https://github.com/Ricardo711/Candy-Magic-App.git
cd Candy-Magic-App
```

### Step 2: Run All Services (Optional: using Docker)

Make sure you have Docker and Docker Compose installed.

```bash
docker-compose up --build
```

Once built:

- 🌐 Frontend: `http://localhost:3000`
- ⚙️ FastAPI ML service: `http://localhost:8000`
- 📡 Node.js backend: `http://localhost:5000`

### Step 3: Run Each Service Manually (Optional)

#### Frontend

```bash
cd frontend
npm install
npm run dev
```

#### FastAPI ML Service

```bash
cd fastapi-service
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

#### Node.js Backend

```bash
cd node-service
npm install
node index.js
```

## 🛠️ Tech Stack

| Layer     | Technologies                             |
|-----------|------------------------------------------|
| Frontend  | React / Next.js                          |
| Backend   | Python, FastAPI, Deep Learning (PyTorch/TensorFlow) |
| API Auth  | Node.js, Express, JWT, MongoDB/PostgreSQL |
| DevOps    | Docker, Git, GitHub                      |

## 📡 API Overview

### FastAPI (ML Service)

| Method | Endpoint   | Description                       |
|--------|------------|-----------------------------------|
| POST   | `/predict` | Returns prediction based on input |

### Node.js Backend

| Method | Endpoint   | Description                       |
|--------|------------|-----------------------------------|
| GET    | `/prices`  | Fetch latest pricing              |
| POST   | `/login`   | Authenticate user                 |

## 📋 TODO List

- [ ] Build and polish UI components
- [ ] Connect FastAPI ML predictions to frontend
- [ ] Set up API Gateway (optional)
- [ ] Add testing and CI/CD (GitHub Actions)
- [ ] Deploy on cloud (Render, Vercel, AWS)

## 👨‍💻 Developer

**Ricardo Alonso Manjarrez Retes**  
GitHub: [@Ricardo711](https://github.com/Ricardo711)

## 📝 License

This project is licensed under the MIT License.


