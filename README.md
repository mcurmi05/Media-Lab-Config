# Ubuntu Server Media Lab Config

This project is a **starter configuration for setting up a home media lab**, primarily centered around **Plex Media Server**. It uses Docker and Docker Compose to deploy and manage various self-hosted services that work together to organize, download, and stream media.

---


This setup includes the following containers:

### 📁 File Browser
A web based file manager used to navigate, edit, and manage media and download directories with ease.

### 🌐 Nginx Proxy Manager
Provides a simple web interface to manage reverse proxies, SSL certificates via Let's Encrypt, and expose internal services securely to the internet.

### 🌊 qBittorrent *(for legal downloads only!)*
A powerful and user friendly torrent client for handling media downloads (only use this to download non pirated media).

### 🎬 Plex Media Server
Streams your organized media collection to multiple devices, with metadata, posters, and sick library views, with users for family use.

### 🖥️ Portainer
A lightweight container management UI to view, manage, and troubleshoot your Docker containers. I've found this especially useful for fixing issues remotely!

### 🧭 Homarr
A beautiful and customizable web dashboard to quickly access and organize all of your media lab services in one place.

---

## 🧱 Requirements

- Any kind of computer (old unused laptops are great). If you want your media server to be running 24/7, best to run something lightweight (I chose Ubuntu Server)
- Docker and docker compose
