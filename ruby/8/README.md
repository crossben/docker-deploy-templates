# 🐳 Ruby on Rails 8 (Pre-release Ready) - Docker Environment

This folder contains a Docker-based setup for **Ruby on Rails 8**, using **Ruby 3.3** and **PostgreSQL 14** — future-proofed for when Rails 8 is officially released.

---

## ⚙️ Stack

| Service | Description        |
|---------|--------------------|
| web     | Ruby 3.3 + Rails 8 |
| db      | PostgreSQL 14      |

---

## 🚀 Getting Started

### 1. Create your Rails 8 app (if not created yet)

```bash
docker-compose run web rails new . --force --database=postgresql
