# 🐳 Ruby on Rails 7 - Docker Environment

This folder contains a minimal Docker-based setup for running **Ruby on Rails 7** using **Ruby 3.2** and **PostgreSQL 14**.

---

## ⚙️ Stack

| Service | Description        |
|---------|--------------------|
| web     | Ruby 3.2 + Rails 7 |
| db      | PostgreSQL 14      |

---

## 🚀 Getting Started

### 1. Create your Rails 7 app (if you haven’t already)

```bash
docker-compose run web rails new . --force --database=postgresql
