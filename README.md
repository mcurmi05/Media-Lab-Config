# Media Lab Config

This project is a **starter config for setting up a home media lab**, primarily centered around a **Plex Media Server**, I've found that Jellyfin is a great alternative but have come back to plex time and time again for small features. It uses Docker and Docker Compose to deploy and manage various self hosted services that work together to organize, download, and stream media. After experimenting with different interfaces and features for roughly 3 months I've found this to be the perfect setup that I have running all the time on my old unused laptop. If anything fails (or my laptop eventually explodes) I can always come back to this repo to rebuild my media setup.

---


This setup includes the following containers:

### 🎬 Plex Media Server
Streams your organized media collection to multiple devices, with metadata, posters, and sick library views, with users for family use.

### 🌐 Nginx Proxy Manager
Provides a simple web interface to manage reverse proxies, SSL certificates via Let's Encrypt, and expose internal services securely to the internet. Consider alternatives to this like using some sort of VPN setup, cloudflare is great for that. I've used this along with domain records to essentially have my own websites for each of my services with SSL encryption.

### 📁 File Browser
A web based file manager used to navigate, edit, and manage media and download directories with ease. If you want to download media remotely you need to be able to move it to a plex recognised media directory once its done so this is great for that sort of task!

### 🌊 qBittorrent *(for legal downloads only!)*
A powerful and user friendly torrent client for handling media downloads (only use this to download non pirated media).

### 🖥️ Portainer
A lightweight container management UI to view, manage, and troubleshoot your Docker containers. I've found this especially useful for fixing issues remotely!

### 🧭 Homarr
A beautiful and customizable web dashboard to quickly access and organize all of your media lab services in one place.

---

## 🧱 Requirements

- Any kind of computer (old unused laptops are great). If you want your media server to be running 24/7, best to run something lightweight (I chose Ubuntu Server, which is a super lightweight barebones linux distribution)
- Docker and docker compose
- Make sure to open ports 80 and 443 on your firewall for this to work (if you prefer not to a VPN setup might be better)
