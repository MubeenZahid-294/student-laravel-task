# 🎓 student-laravel-task
A Laravel-based project demonstrating structured database design and automated data generation using **Migrations**, **Factories**, and **Seeders**.

## 🚀 Overview

This project showcases how Laravel simplifies backend development by providing powerful tools for database management and data seeding. The system creates a `students` table and populates it with realistic fake data using Faker.

## ⚙️ Features

- 📌 Database schema creation using Laravel **Migrations**
- 🏭 Automated data generation using **Factories**
- 🌱 Bulk data insertion using **Seeders**
- 🎲 Realistic dummy data powered by **Faker**
- 🛢️ MySQL database integration via XAMPP


## 🛠️ Tech Stack

- **Laravel (PHP Framework)**
- **PHP**
- **MySQL**
- **Faker Library**


## 🧩 Database Structure

The `students` table includes:

- `id` (Primary Key)
- `name` (String)
- `email` (Unique)
- `age` (Integer)
- `created_at` / `updated_at` (Timestamps)

## ⚡ Setup Instructions

```bash
git clone <your-repo-link>
cd student-project
composer install
cp .env.example .env
php artisan key:generate


### **Configure Database in `.env`**
```env
DB_DATABASE=student_project
DB_USERNAME=root
DB_PASSWORD=

### Run Migrations and Seeder
php artisan migrate:fresh
php artisan db:seed --class=StudentSeeder
