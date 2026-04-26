# DevSecOps AI Code Reviewer

A complete DevOps project demonstrating CI/CD pipeline with Jenkins, Docker containerization, and AI-powered code security analysis.

## 🎯 Project Purpose (DevOps Demo)

This project demonstrates:
- ✅ **Build Process**: Automated builds with Jenkins
- ✅ **Dockerization**: Multi-container application setup
- ✅ **CI/CD Pipeline**: Complete pipeline from code to deployment
- ✅ **Application**: Working AI code scanner with UI + Backend
- ✅ **Git Integration**: Full source code management

## 🚀 Quick Start

### Option 1: Docker (RECOMMENDED for Demo)

```bash
# Build and run with Docker Compose
docker-compose up --build

# Access application
http://localhost
```

### Option 2: Local Development

**Step 1: Install Dependencies**
```bash
# Install frontend dependencies
pnpm install

# Install backend dependencies
cd backend
pip install -r requirements.txt
cd ..
```

**Step 2: Start Backend (Terminal 1)**
```bash
cd backend
python app.py
```

**Step 3: Start Frontend (Terminal 2)**
```bash
pnpm run dev
```

**Step 4: Open Browser**
```
http://localhost:5173
```

See **[LOCAL_DEVELOPMENT.md](./LOCAL_DEVELOPMENT.md)** for detailed instructions.

## 📦 Tech Stack

**Frontend:**
- React + TypeScript
- Tailwind CSS v4
- Motion (Framer Motion)

**Backend:**
- Python Flask
- Google Gemini AI
- SQLite Database

**DevOps:**
- Docker & Docker Compose
- Jenkins CI/CD
- Nginx (Production)

## 🔧 Jenkins Pipeline

The `Jenkinsfile` defines stages:
1. Checkout code from Git
2. Build Backend Docker image
3. Build Frontend Docker image
4. List Docker images (verification)
5. Deploy with Docker Compose
6. Verify deployment

## 📊 Features

- 🔍 **AI Code Analysis**: Detects security vulnerabilities, bugs, and code smells
- 🛡️ **Security Scanning**: Powered by Google Gemini 1.5 Flash
- 📈 **Scan History**: SQLite database tracks all analyses
- ⚡ **Real-time Results**: Live AI feedback
- 🎨 **Modern UI**: Clean, minimalist interface

## 📖 Documentation

- **[DEVOPS_DEMO_GUIDE.md](./DEVOPS_DEMO_GUIDE.md)** - Complete demo instructions
- **[SETUP.md](./SETUP.md)** - Detailed setup guide

## 🐳 Docker Commands

```bash
# Build images
docker-compose build

# Run containers
docker-compose up -d

# View logs
docker-compose logs -f

# Stop containers
docker-compose down

# List images
docker images | grep devsecops
```

## 📁 Project Structure

```
.
├── backend/
│   ├── app.py              # Flask API
│   ├── Dockerfile          # Backend container
│   └── requirements.txt
├── src/                    # React frontend
├── Dockerfile              # Frontend container
├── docker-compose.yml      # Multi-container setup
├── Jenkinsfile            # CI/CD pipeline
└── nginx.conf             # Production server config
```

## 🎬 Demo Checklist

- [ ] Application runs and analyzes code
- [ ] Code pushed to GitHub with Dockerfiles
- [ ] Jenkins pipeline executes successfully
- [ ] Docker images created (`docker images`)
- [ ] End-to-end flow: Git → Jenkins → Docker → Running app
- [ ] Application runs in Docker containers (not local)

## 🔑 API Endpoints

- `POST /api/scan` - Analyze code snippet
- `GET /api/history` - Retrieve scan history
- `GET /api/stats` - Get statistics

## 🌐 Access Points

- **Frontend (Docker)**: http://localhost
- **Backend API (Docker)**: http://localhost:5000
- **Backend (Local)**: http://localhost:5000

## 📝 License

Educational DevOps Project
# aicodereviewerprojectdsce
# devopsaicodereview
# devopsaicodereview
