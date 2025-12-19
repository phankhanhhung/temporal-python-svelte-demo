# Temporal Python + Svelte Demo

A demo application combining Temporal.io (Python) backend with a Svelte frontend.

## Project Structure

- `backend/` - Python Temporal workflow and activities
- `worker/` - Temporal Python worker
- `frontend/` - Svelte frontend application
- `docker-compose.yml` - Local development environment setup

## Prerequisites

- Docker and Docker Compose
- Python 3.9+
- Node.js 18+

## Getting Started

### Start Temporal Server

```bash
docker-compose up -d
```

### Start the Worker

```bash
cd worker
pip install -r requirements.txt
python worker.py
```

### Start the Backend API

```bash
cd backend
pip install -r requirements.txt
python main.py
```

### Start the Frontend

```bash
cd frontend
npm install
npm run dev
```

## Development

The frontend will be available at `http://localhost:5173`
The backend API will be available at `http://localhost:8000`
Temporal Web UI at `http://localhost:8080`

## License

MIT