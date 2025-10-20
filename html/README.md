# 🐳 Static HTML Site - Docker Environment

This setup uses **Nginx** in a Docker container to serve a basic **static HTML/CSS/JS website**.

---

## ⚙️ Stack

| Service | Description |
|---------|-------------|
| web     | Nginx (serving static files) |

---

## 🚀 Getting Started

### 1. Create your HTML project

Include a basic `index.html` file at the root of the folder, like:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Hello Docker</title>
  </head>
  <body>
    <h1>Welcome to Dockerized HTML!</h1>
  </body>
</html>
