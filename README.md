# My Tasks — Laravel Foundation

The authenticated foundation of **My Tasks**, a personal task-management app built with Laravel 12. This repository ships the complete account and access layer the product is built on — registration, login, email verification and profile management — with a protected dashboard ready for the task modules.

## What's implemented

- **Full authentication** — registration, login, logout, password reset and email verification (Laravel Breeze)
- **Livewire-powered profile** — update profile information, change password, and delete account, all as reactive Livewire/Volt components (no page reloads)
- **Protected dashboard** — authenticated, email-verified area behind route middleware
- **Modern Laravel stack** — Eloquent ORM, migrations, Blade views, Vite + Tailwind CSS asset pipeline
- **Testing setup** — PHPUnit configuration and feature-test scaffolding included

## Tech stack

- **Backend:** PHP 8.2+ · Laravel 12 · MySQL (Eloquent ORM)
- **Frontend:** Blade · Livewire 3 / Volt · Alpine.js · Tailwind CSS
- **Auth:** Laravel Breeze (Livewire edition)
- **Tooling:** Vite · Composer · PHPUnit

## Getting started

```bash
# 1. Install dependencies
composer install
npm install

# 2. Configure environment
cp .env.example .env
php artisan key:generate
# set DB_* values in .env for your MySQL database

# 3. Migrate
php artisan migrate

# 4. Run
php artisan serve        # http://localhost:8000
npm run dev              # asset pipeline (separate terminal)
```

## Project status

The authentication and account foundation is complete. Task management (task CRUD, lists and organisation) is the next layer, built on top of this base.

## License

MIT
