# 🧠 Personal Habit Tracker App

A modern Flutter-based habit tracking application designed to help users build consistency, track progress, and develop positive routines through a clean UI and structured data tracking.

---

## 🚀 Overview

The Personal Habit Tracker App enables users to create, manage, and monitor their daily habits efficiently. It focuses on simplicity, performance, and scalability while leveraging modern Flutter architecture and backend integration.

The app is designed to:

* Track daily habit completion
* Store logs and progress over time
* Provide insights into user consistency
* Support authentication and user-based data

---

## ✨ Features

### 🔐 Authentication

* Secure user authentication (Email / OAuth)
* Session persistence
* User-specific data isolation

### 📋 Habit Management

* Create, update, and delete habits
* Assign habits to specific users
* Flexible habit structure (daily tracking)

### ✅ Habit Logs

* Mark habits as completed
* Store completion logs with timestamps
* Track completion history

### 📊 Progress Tracking

* Count completed logs per habit
* Aggregate statistics (e.g., total completed habits)
* Prepare data for charts and analytics

### 🔄 Real-time Data Handling

* Sync habit logs with backend
* Reactive UI updates

---

## 🏗️ Architecture

The project follows a clean and scalable architecture:

```
lib/
├── core/            # shared utilities, constants
├── data/            # models, data sources
├── domain/          # business logic (entities/use cases)
├── presentation/    # UI + controllers (GetX / Bloc)
├── services/        # API / Supabase integration
└── main.dart
```

---

## 🛠️ Tech Stack

* **Flutter** – Cross-platform UI framework
* **Dart** – Programming language
* **Supabase** – Backend (Auth + Database + Realtime)
* **PostgreSQL** – Relational database
* **GetX / Bloc** – State management

---

## 📱 App Screens

<img width="502" height="820" alt="Screenshot 1447-11-30 at 8 49 19 am" src="https://github.com/user-attachments/assets/eba9b24a-ae92-4050-b2ad-a153b8a50778" />
<img width="502" height="820" alt="Screenshot 1447-11-30 at 8 49 50 am" src="https://github.com/user-attachments/assets/cc06350d-4ffd-4573-a81a-417c992b23be" />
<img width="642" height="820" alt="WhatsApp Image 1447-11-03 at 22 39 18" src="https://github.com/user-attachments/assets/6cd6abab-4247-4fec-bfca-4d41561f9968" />




---

## 🗄️ Database Design

### Users Table

* Stores user profile data
* Linked to `auth.users`

### Habits Table

* Each habit belongs to a user

### Habit Logs Table

* Stores completion logs
* Linked to habits

---

## 🔗 Relationships

* One User → Many Habits
* One Habit → Many Logs

---

## 📱 Getting Started

### Prerequisites

* Flutter SDK
* Supabase project
* Android Studio / VS Code

---

### Installation

```bash
git clone <repo-link>
cd habit_tracker_app_flutter
flutter pub get
```

---

### Run the App

```bash
flutter run
```

---

## 🔑 Environment Setup

Create a `.env` file and add:

```
SUPABASE_URL=your_url
SUPABASE_ANON_KEY=your_key
```

