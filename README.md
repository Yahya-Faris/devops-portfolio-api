# Docker Practice: Node.js API

This is a practice project for my DevOps learning journey. I built a simple Node API and containerized it using Docker best practices.

### What I did in this project:
- Used **Multi-stage builds** to keep the image small.
- Used `node:20-alpine` as a lightweight base image.
- Set up a non-root user for better security.
- Ordered the `Dockerfile` steps to optimize layer caching.
- Pushed the final image to GitHub Container Registry (GHCR).

### Next steps:
Deploying this container on an AWS EC2 instance.

### Run it locally:
```bash
docker run -p 3000:3000 -d ghcr.io/yahya-faris/devops-portfolio-api:v1
Yahya Faris

Business Information Technology Student learning DevOps & Linux.