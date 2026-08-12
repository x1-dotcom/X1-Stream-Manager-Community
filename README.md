# 🚀 X1 Stream Manager Community v1.0.0
### Modern Adult IPTV Control Center, Live Stream Relay & Customer Line Manager

---

## 📌 Overview

**X1 Stream Manager Community v1.0.0** is a powerful, lightweight, self-hosted IPTV management platform and live stream resolver. It allows webmasters, IPTV resellers, and community administrators to manage, stream, and deliver 40 high-demand live adult television channels with **zero buffer, instant sub-200ms token resolution, and seamless client compatibility**.

Whether you want to offer interactive live streaming on your website or distribute managed M3U playlists to clients using IPTV applications (VLC, Tivimate, Smart IPTV, Kodi, Enigma2, or Xtream Codes apps), **X1 Stream Manager** delivers a complete out-of-the-box solution.

---

## 🔥 Key Features

- ⚡ **Instant Live Stream Resolver Engine**: Sub-200ms automated token extraction (`wmsAuthSign`) directly from live remote sources.
- 🛡️ **Zero-CORS & Anti-Block Stream Proxy (`stream.php`)**: Built-in server-side HLS proxy bypasses browser CORS blocks, referrer checks, and `X-Frame-Options` restrictions.
- 📺 **Dual-Mode Interactive Web Player (`list.php` & `line.php`)**: Watch channels live in your browser using an embedded HLS player, or export formatted `#EXTM3U` playlists.
- 👥 **Line & Customer Access Management**: Create user accounts, generate expiring line access tokens, assign specific channel packages per line, and track line activity.
- 📺 **Xtream Codes API Compatibility (`player_api.php`)**: Built-in API emulator for seamless integration with Smarters, Tivimate, and IPTV boxes (`/player_api.php?username=...&password=...`).
- 🎨 **Sleek Glassmorphism Control Panel**: Modern dark UI with live health badges, latency monitors, and quick M3U link generators.
- 🚀 **1-Click First-Run Installer (`setup.php`)**: Self-installs upon first visit. No pre-configured database or complex setup required.

---

## 📋 System Requirements

To host **X1 Stream Manager Community**, your web server must meet the following minimum requirements:

- **Web Server**: Nginx, Apache, Caddy, or PHP Built-in Server.
- **PHP Version**: PHP 8.0, 8.1, 8.2, or 8.3.
- **PHP Extensions**: `ext-curl`, `ext-json`, `ext-mbstring`, `ext-zlib`, `ext-openssl`.
- **File Permissions**: Write access to the `data/` directory (`chmod 775`).

---

## 🛠️ Step-by-Step Installation Guide

### Step 1: Upload Files to Server
1. Download the release package (`X1_Stream_Manager_v1.0.0.zip`).
2. Upload and extract the files to your web server root directory (e.g., `/var/www/html/` or `public_html/`).

### Step 2: Set Directory Permissions
Ensure the web server has write permission for the `data/` folder:
```bash
chmod -R 775 data/
