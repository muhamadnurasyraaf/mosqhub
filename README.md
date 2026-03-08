# MosqHub 🕌
> Mosque Management System — currently in production in Malaysia

A fullstack web platform that digitalizes mosque operations for AJK (committee) administrators and Kariah (congregation) members. Replaces manual, paper-based processes with a centralized system.

---

## 🧩 Modules

| Module | Description |
|--------|-------------|
| Kariah | Member registry and management |
| Khairiat | Funeral/bereavement fund contributions and payouts |
| Events | Mosque event scheduling and announcements |
| Infrastructure Rental | Facility booking management |
| Finance | Financial records and reporting |
| AJK | Committee member management |

---

## 🏗️ Architecture
```
Client (Web)          Client (Mobile)
     │                      │
Next.js Admin         Flutter App
     │                      │
     └──────────┬───────────┘
                │
          Go REST API
          (Gin + GORM)
                │
          PostgreSQL
          (Supabase)
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | Go, Gin, GORM |
| Web Frontend | Next.js, TailwindCSS |
| Mobile | Flutter |
| Database | PostgreSQL (Supabase) |
| Server | GCP VM, nginx, PM2 |
| DNS & SSL | Cloudflare |
| Firewall | UFW |

---

## ⚙️ Infrastructure

Deployed on a cost-efficient GCP VM:

- **nginx** — reverse proxy, routing, SSL termination
- **Cloudflare** — DNS management and SSL certificates
- **PM2** — Go process management and auto-restart on crash
- **UFW** — firewall and port management
- **Supabase** — managed PostgreSQL with minimal overhead

---

## 👥 Users

- **AJK Admin** — manages mosque operations via web dashboard
- **Kariah Members** — congregation members via Flutter mobile app

---

## 📌 Status

`Production` — actively serving a mosque in Malaysia
