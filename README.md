# 🚀 Nginx with Docker Compose (Live HTML Update using Volume Mount)

This project demonstrates how to run **Nginx using Docker Compose** and serve a static website where **changes in `index.html` are reflected instantly** in the browser using **bind mounts (volumes)**.

---

## 📂 Project Structure

```text
.
├── compose.yml
└── html
    └── index.html
---

 ## Volume Mount Explanation

./html → Host machine folder
/usr/share/nginx/html → Default Nginx web root inside container

./html is not created by default — you must create it manually

/usr/share/nginx/html already exists inside the Nginx image

How to Run
1️⃣ Start the container
docker compose up -d

2️⃣ Open in browser
http://localhost:8080
