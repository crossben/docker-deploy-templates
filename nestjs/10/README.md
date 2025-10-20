
---

## 📁 `/nestjs/10/README.md`

```md
# 🐳 NestJS 10 — Dockerized Setup

This folder contains a Docker environment to run **NestJS 10**, with optional PostgreSQL database support and full hot-reload capability for development.

> ✅ NestJS 10 introduces improved performance, enhanced decorators, and better support for modular monoliths and microservices.

---

## ⚙️ Stack

| Service | Description                 |
|---------|-----------------------------|
| web     | Node.js 18 + NestJS 10      |
| db      | *(optional)* PostgreSQL 14  |

---

## 🚀 Getting Started

# Build the Next.js app this should work unless you have a custom build script

### 1. Navigate into the NestJS 10 project folder

```bash

docker-compose up -d --build
