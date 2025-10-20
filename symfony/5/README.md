
---

### 📁 `/symfony/5/README.md`

```md
# 🐳 Symfony 5 - Dockerized Environment

This folder provides a Dockerized development setup for **Symfony 5**, still useful for maintaining legacy or long-running projects.

> ⚠️ Symfony 5 is no longer actively maintained — use only for legacy support.

---

## 🧱 Docker Components

| Service | Description             |
|---------|-------------------------|
| web     | Apache + PHP 7.4/8.0    |
| db      | MySQL 5.7 or 8.0        |

---

## 🔥 Quick Start

### Run this command from the root of your project folder:

```bash

composer create-project symfony/skeleton:^5.0 replace-with-your-app-name

cd replace-with-your-app-name

docker-compose up -d --build
