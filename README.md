# 3x-ui 3D Subscription Template (YuzuNet Edition)

A modern, self-contained subscription page template for [3x-ui](https://github.com/MHSanaei/3x-ui) — glassmorphism cards, 3D tilt, animated 3D background, circular usage gauge, QR code, one-tap app import, and full **Persian (فارسی) / English** support with RTL/LTR switching.

![Showcase](showcase.png)

## Features

- 🌐 FA / EN toggle (saved in the browser), automatic RTL/LTR
- 🌓 Auto dark / light theme (follows the device)
- 🧊 3D floating background scene + mouse-tilt cards (pure CSS/JS, no libraries)
- 📊 Circular usage gauge, days-remaining countdown, upload/download/total/remaining stats
- 📅 Jalali (شمسی) dates in Persian mode, Gregorian in English
- 🔗 Copy buttons for subscription / JSON / Clash links + QR code (generator embedded — works offline/with blocked CDNs)
- 📱 One-tap import: v2rayNG, Hiddify, Streisand, Shadowrocket, Happ, FlClash (editable list)
- 🟢 Live online/offline status badge — auto-refreshes every 30s via the panel's `?format=info` endpoint
- 📢 Announcement banner, support button, per-config list with copy
- 📦 Single `index.html` file — no assets, no build step

## Install

> **Requires 3x-ui v3.3.0+** (custom subscription templates were added in [v3.3.0](https://github.com/MHSanaei/3x-ui/releases/tag/v3.3.0)). The live online/offline badge uses the `?format=info` endpoint from newer builds — on older panels the badge simply shows the render-time status.

**One-liner** — paste this on your server:

```bash
sudo mkdir -p /etc/3x-ui/sub_templates/3x-ui-sub-Yuzutemplate && sudo curl -fsSL https://raw.githubusercontent.com/sadybe/3x-ui-sub-Yuzutemplate/main/index.html -o /etc/3x-ui/sub_templates/3x-ui-sub-Yuzutemplate/index.html && sudo chmod 755 /etc/3x-ui/sub_templates /etc/3x-ui/sub_templates/3x-ui-sub-Yuzutemplate && sudo chmod 644 /etc/3x-ui/sub_templates/3x-ui-sub-Yuzutemplate/index.html
