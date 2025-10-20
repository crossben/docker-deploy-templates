<p align="center">
    <img src="https://cdn.simpleicons.org/laravel/FF2D20" alt="Laravel" width="40" />
    <img src="https://cdn.simpleicons.org/symfony/FFFFFF" alt="Symfony" width="40" />
    <img src="https://cdn.simpleicons.org/react/61DAFB" alt="React" width="40" />
    <img src="https://cdn.simpleicons.org/nextdotjs/FFFFFF" alt="Next.js" width="40" />
    <img src="https://cdn.simpleicons.org/nestjs/E0234E" alt="NestJS" width="40" />
    <img src="https://cdn.simpleicons.org/astro/FF5D01" alt="Astro" width="40" />
    <img src="https://cdn.simpleicons.org/vuejs/4FC08D" alt="Vue.js" width="40" />
    <img src="https://cdn.simpleicons.org/express/000000" alt="Express.js" width="40" />
    <img src="https://cdn.simpleicons.org/django/092E20" alt="Django" width="40" />
    <img src="https://cdn.simpleicons.org/rubyonrails/CC0000" alt="Ruby on Rails" width="40" />
</p>

# 🚀 Docker Boilerplates for Your Web Projects

This repository provides **Docker configuration files only** — `Dockerfile` and `docker-compose.yml` — for various popular web frameworks and versions.

---

## ⚠️ Important

> **Note:** This repo does **not** include any application source code.

To use these Docker templates:

1. Create your own project folder for the framework/version you want.
2. Copy the corresponding `Dockerfile` and `docker-compose.yml` from this repo into your project folder.
3. Customize as needed (e.g., add your app source code, `.env` files).
4. Use Docker to build and run your project container.

---

## 🐳 What You Need

### 1. Install Docker

- **Windows / macOS**: [Docker Desktop](https://www.docker.com/products/docker-desktop)
- **Linux**:

  ```bash
  sudo apt update
  sudo apt install docker.io docker-compose -y
  sudo systemctl start docker
  sudo systemctl enable docker



## 📂 Supported Frameworks and Versions

| Framework     | Versions                                   | Folder Path            |
|---------------|--------------------------------------------|------------------------|
| Laravel       | [10](laravel/10), [11](laravel/11), [12](laravel/12) | [`/laravel/`](laravel)     |
| Symfony       | [5](symfony/5), [6](symfony/6), [7](symfony/7)       | [`/symfony/`](symfony)     |
| React         | [18](react/18), [19](react/19)                     | [`/react/`](react)         |
| Next.js       | [13](nextjs/13), [14](nextjs/14)                   | [`/nextjs/`](nextjs)       |
| NestJS        | [9](nestjs/9), [10](nestjs/10)                     | [`/nestjs/`](nestjs)       |
| Astro         | [4](astro/4)                                      | [`/astro/`](astro)         |
| Vue.js        | [2](vue/2), [3](vue/3)                            | [`/vue/`](vue)             |
| Express.js    | [4](express/4), [5](express/5) *(future-proof)*   | [`/express/`](express)     |
| Django        | [4](django/4), [5](django/5)                      | [`/django/`](django)       |
| Ruby on Rails | [7](ruby/7), [8](ruby/8) *(pre-release ready)*  | [`/ruby/`](ruby)         |




