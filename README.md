# 🌐 Nginx Reverse Proxy

This repository provides a simple and secure **Nginx reverse proxy** setup using Docker Compose.  
It is designed to serve as an HTTPS entry point for applications running on the same Docker network (`shared-net`).

---

## 🧱 Overview

This setup runs an **Nginx** container that:
- Listens on port **443** (HTTPS)
- Uses a **custom Nginx configuration**
- Loads **SSL certificates** from your local machine (mounted into the container)
- Connects to the shared Docker network (`shared-net`) to route traffic to other services (e.g., APIs, web apps)
