# 🤖 Agent Documentation - Admin Digital

> Dokumentasi AI untuk pengembangan project Admin Digital

---

## 📋 Project Overview

| Item              | Detail                                      |
| ----------------- | ------------------------------------------- |
| **Nama Project**  | Admin Digital                               |
| **Deskripsi**     | Website admin panel untuk manajemen digital |
| **Tanggal Mulai** | 1 Februari 2026                             |
| **Status**        | 🟡 In Development                           |

---

## 🛠️ Tech Stack

### Backend

- **Framework**: Laravel v12.49.0
- **PHP Version**: 8.4.12
- **Admin Panel**: Filament v3 (akan diinstall)
- **Database**: SQLite (development) / MySQL (production)

### Frontend

- **CSS Framework**: Tailwind CSS
- **Build Tool**: Vite
- **JavaScript**: Vanilla JS / Alpine.js (via Filament)

### Development Tools

- **Package Manager**: Composer 2.8.11
- **Node Package Manager**: NPM
- **Version Control**: Git

---

## 📅 Development Log

### 1 Februari 2026

#### ✅ Completed

- [x] Inisialisasi project Laravel v12.49.0
- [x] Setup environment development
- [x] Database SQLite sudah di-migrate (users, cache, jobs tables)
- [x] Server development berjalan di `http://127.0.0.1:8000`

#### 🔄 In Progress

- [ ] Install Filament v3 untuk admin panel
- [ ] Setup Tailwind CSS untuk tampilan depan

#### 📝 Pending

- [ ] Konfigurasi admin panel
- [ ] Design tampilan depan website
- [ ] Setup authentication
- [ ] Membuat fitur-fitur admin

---

## 📁 Project Structure

```
admin-digital/
├── app/                    # Application logic
│   ├── Http/
│   │   └── Controllers/    # Controllers
│   ├── Models/             # Eloquent models
│   └── Providers/          # Service providers
├── bootstrap/              # Framework bootstrap
├── config/                 # Configuration files
├── database/
│   ├── factories/          # Model factories
│   ├── migrations/         # Database migrations
│   └── seeders/            # Database seeders
├── public/                 # Public assets
├── resources/
│   ├── css/               # Stylesheets
│   ├── js/                # JavaScript files
│   └── views/             # Blade templates
├── routes/
│   ├── web.php            # Web routes
│   └── console.php        # Console routes
├── storage/               # Storage (logs, cache, uploads)
├── tests/                 # Test files
├── vendor/                # Composer dependencies
├── .env                   # Environment configuration
├── artisan                # Laravel CLI
├── composer.json          # PHP dependencies
├── package.json           # Node dependencies
└── vite.config.js         # Vite configuration
```

---

## 🚀 Commands Reference

### Development Server

```bash
# Start Laravel server
php artisan serve

# Start Vite dev server (frontend assets)
npm run dev

# Run both (in separate terminals)
php artisan serve & npm run dev
```

### Database

```bash
# Run migrations
php artisan migrate

# Fresh migration (reset & re-run)
php artisan migrate:fresh

# Seed database
php artisan db:seed
```

### Artisan Commands

```bash
# Create controller
php artisan make:controller NamaController

# Create model with migration
php artisan make:model NamaModel -m

# Create Filament resource
php artisan make:filament-resource NamaResource

# Clear cache
php artisan cache:clear
php artisan config:clear
php artisan view:clear
```

---

## 🔐 Environment Variables

File `.env` berisi konfigurasi penting:

```env
APP_NAME="Admin Digital"
APP_ENV=local
APP_DEBUG=true
APP_URL=http://localhost:8000

DB_CONNECTION=sqlite
# DB_CONNECTION=mysql
# DB_HOST=127.0.0.1
# DB_PORT=3306
# DB_DATABASE=admin_digital
# DB_USERNAME=root
# DB_PASSWORD=
```

---

## 📌 Notes untuk AI Agent

1. **Filament Version**: Gunakan Filament v3, BUKAN v4 (compatibility issues)
2. **Tailwind CSS**: Digunakan untuk tampilan depan website (landing page, dll)
3. **Database Development**: Menggunakan SQLite untuk kemudahan development
4. **Admin Panel Path**: Akan di-setup di `/admin`

---

## 🎯 Fitur yang Akan Dikembangkan

### Phase 1 - Foundation

- [ ] Setup Filament v3 admin panel
- [ ] Konfigurasi Tailwind CSS
- [ ] User management system
- [ ] Basic authentication

### Phase 2 - Core Features

- [ ] Dashboard admin
- [ ] CRUD operations
- [ ] File management
- [ ] Settings management

### Phase 3 - Enhancement

- [ ] Reporting & analytics
- [ ] Notifications system
- [ ] API endpoints
- [ ] Advanced permissions (roles)

---

_Dokumentasi ini otomatis di-update oleh AI Agent_
