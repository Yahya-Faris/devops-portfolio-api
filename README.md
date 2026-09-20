# Docker Practice: Node.js API

This is a practice project for my DevOps learning journey. I built a simple Node API, containerized it using Docker best practices, and deployed it to AWS.

### Live Demo:
https://yahya-api.duckdns.org

### What I did in this project:
- Used **Multi-stage builds** to keep the image small.
- Used `node:20-alpine` as a lightweight base image.
- Set up a non-root user for better security.
- Ordered the `Dockerfile` steps to optimize layer caching.
- Pushed the final image to GitHub Container Registry (GHCR).
- Deployed the container on an AWS EC2 instance (Ubuntu).
- Set up Nginx as a reverse proxy to route traffic.
- Added HTTPS using DuckDNS and Let's Encrypt (Certbot).

### Run it locally:
```bash
docker run -p 3000:3000 -d ghcr.io/yahya-faris/devops-portfolio-api:v1
Yahya Faris
Business Information Technology Student learning DevOps & Linux.