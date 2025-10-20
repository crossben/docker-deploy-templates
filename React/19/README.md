# ⚛️ React 19 (Beta) — Docker Setup

This folder contains a **Dockerized environment for React 19**, the latest version (currently in beta as of 2025), designed to help you get started quickly using Docker.

> 📦 This setup includes only the `Dockerfile` and `docker-compose.yml` — you need to create your React app separately and copy these files into it.

---

## 🚀 Quick Start

### 1. Create a new React 19 project

If you don't already have a React 19 app, you can create one like this:

#### Option 1: Using `create-react-app` (if available)

```bash

npx create-react-app@next my-react19-app
cd my-react19-app


docker-compose up -d --build