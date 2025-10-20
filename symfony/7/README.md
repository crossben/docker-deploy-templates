# 🐳 Symfony 7 - Dockerized Environment

This folder provides a Docker-ready setup for **Symfony 7** — the latest version with modern PHP 8.2+ features.

> ✅ Symfony 7 requires **PHP ≥ 8.2** and is ideal for long-term projects using the latest Symfony ecosystem.

---

## 🧱 Docker Components

| Service | Description             |
|---------|-------------------------|
| web     | Apache + PHP 8.2/8.3    |
| db      | MySQL 8.0               |

---

## 🔥 Quick Start

### Run this command from the root of your project folder:

```bash

composer create-project symfony/skeleton:^7.0 replace-with-your-app-name

cd replace-with-your-app-name

docker-compose up -d --build
