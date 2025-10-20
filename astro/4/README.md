# 🪐 Astro 4 — Dockerized Setup

This folder contains a **Docker environment for Astro 4** — a fast, modern static site builder.

> 📦 This setup includes only the Dockerfile and docker-compose.yml — you must create your Astro project separately and copy these files into it.

---

## 🚀 Quick Start

### 1. Create a new Astro project

If you haven’t already:

```bash
npm create astro@latest
cd my-astro-app

docker-compose up -d --build
