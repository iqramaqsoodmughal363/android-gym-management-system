# 🏋️ Gym Management System

<p align="center">
  <b>A complete, all-in-one solution for managing your fitness center.</b>
</p>

<p align="center">
  <em>"A comprehensive Android application built in Java to manage gym operations, including memberships, payments, attendance, workout routines, and health tracking."</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F-red" alt="Made with Love">
  <img src="https://img.shields.io/badge/Platform-Android-green" alt="Platform">
  <img src="https://img.shields.io/badge/Language-Java-orange" alt="Language">
  <img src="https://img.shields.io/badge/Backend-Firebase-yellow" alt="Firebase">
  <img src="https://img.shields.io/badge/Status-Complete-success" alt="Status">
</p>

---

## 📋 Overview

**Gym Management System** is a full-featured, enterprise-level Android application designed to digitize and streamline the operations of a fitness center. Built in **Java**, this app provides a seamless experience for gym administrators to track members, manage payments, log attendance, and monitor the health and workout progress of every member.

The app features a modular architecture with dedicated Activities, Adapters, Fragments, and Models, ensuring scalability and clean code practices.

---

## ✨ Key Features

* **👥 Member Management:** Add, edit, view details, and list all gym members (`AddMemberActivity`, `MembersListActivity`, `MemberDetailActivity`).
* **💳 Payment Tracking:** Record new payments and view complete payment histories for each member (`RecordPaymentActivity`, `PaymentHistoryActivity`).
* **📅 Attendance System:** Mark daily attendance and view historical attendance records (`AttendanceActivity`, `AttendanceHistoryActivity`).
* **🏋️ Workout Routines:** Create customized workout plans for members and view assigned routines (`AddWorkoutRoutineActivity`, `ViewWorkoutActivity`).
* **🥗 Diet Plans:** Assign and track diet plans (`AddDietPlanActivity`, `ViewDietPlanActivity`).
* **❤️ Health Records:** Log vital health metrics and view historical data with charts (`AddHealthRecordActivity`, `HealthHistoryActivity`).
* **📊 Dashboard:** A centralized home screen for quick insights into gym operations (`DashboardActivity`).
* **🔔 Automated Notifications:** Uses `WorkManager` (`NotificationWorker`) to send timely alerts (e.g., expiring memberships).
* **📤 Data Export:** Built-in `ExportHelper` to export member or payment data.
* **🔥 Firebase Integration:** Includes `google-services.json` indicating Firebase Authentication or Firestore integration.

---

## 🛠️ Tech Stack

| Category | Tools / Technologies |
|---|---|
| **Language** | Java |
| **IDE** | Android Studio |
| **Architecture** | Activity-based with Fragments & Adapters |
| **Backend / Auth** | Firebase (via Google Services) |
| **Background Tasks** | `WorkManager` (for notifications) |
| **UI Components** | RecyclerView, Spinner, Custom Dialogs, Charts |
| **Data Handling** | Custom Models (User, Member, Payment, etc.) |

---

## 📂 Project Structure

```text
android-gym-management-system/
│
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/gymmanagement/app/
│   │   │   │   ├── activities/              # All UI Screens
│   │   │   │   │   ├── LoginActivity.java
│   │   │   │   │   ├── DashboardActivity.java
│   │   │   │   │   ├── MembersListActivity.java
│   │   │   │   │   ├── RecordPaymentActivity.java
│   │   │   │   │   └── ... (other activities)
│   │   │   │   ├── adapters/                # RecyclerView Adapters
│   │   │   │   ├── fragments/               # UI Fragments (Health Charts)
│   │   │   │   ├── models/                  # Data Objects
│   │   │   │   │   ├── Member.java
│   │   │   │   │   ├── Payment.java
│   │   │   │   │   └── ... (other models)
│   │   │   │   └── utils/                   # Helper Classes
│   │   │   │       ├── ExportHelper.java
│   │   │   │       └── NotificationHelper.java
│   │   │   ├── res/
│   │   │   │   ├── drawable/                # Custom Icons & Badges
│   │   │   │   ├── layout/                  # Activity & Item Layouts
│   │   │   │   ├── mipmap/                  # App Icons
│   │   │   │   └── values/                  # Colors, Strings, Arrays, Themes
│   │   │   └── AndroidManifest.xml
│   │   └── google-services.json             # Firebase Configuration
│   └── build.gradle
├── build.gradle
├── settings.gradle
└── README.md
```

---

## 🚀 How to Build and Run

### Prerequisites
* **Android Studio** (Latest Version)
* **JDK 11** or higher
* **Android SDK** (API 24+)
* **Firebase Account** (Since `google-services.json` is included, ensure Firebase is set up in your Google Console).

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/iqramaaqsoodmughal363/android-gym-management-system.git
   ```
2. **Open in Android Studio**
   Open Android Studio → **File** → **Open** → Select the project folder.
3. **Sync Gradle**
   Wait for Gradle to sync. Click **"Sync Now"** if prompted.
4. **Build and Run**
   Connect your Android device or start an emulator, then click the **Run** button (green play icon).

---

## ⚙️ How It Works (Behind the Scenes)

### 1. Modular Activity Architecture
Every major feature has its own dedicated Activity (e.g., `AddMemberActivity` for adding a member, `AttendanceActivity` for marking attendance). This keeps the app organized and easy to navigate.

### 2. Data Models & Adapters
The app uses custom Java classes (`Member`, `Payment`, `WorkoutLog`) as data models. These models are bound to the UI using custom `RecyclerView.Adapters` (like `MemberAdapter`) for smooth scrolling and data display.

### 3. Background Tasks (`NotificationWorker.java`)
Using Android's `WorkManager` API, the app runs background tasks to check for expiring memberships and automatically push notifications to the user, even if the app is closed.

### 4. Health Tracking & Charts
The `fragment_health_chart.xml` suggests the use of a charting library (like MPAndroidChart) to visualize member health records (weight, BMI, etc.) over time.

---

## 🎯 Key Takeaways

* **Complete Solution:** A real-world app that solves actual business problems for gym owners.
* **Advanced Android Concepts:** Demonstrates `WorkManager`, Fragments, Custom Dialogs, and Data Exporting.
* **Clean Code:** Proper package structure (`activities`, `models`, `adapters`, `utils`).
* **Firebase Ready:** Built with cloud integration in mind.

---

## 👩‍💻 Author

**Iqra Maqsood Mughal**

*Software Engineer · Full-Stack Developer · Code Craftsman · Android App Developer · Problem Solver 🚀*

```javascript
const codeIsLife = "Code is life";
while (true) { 
    learn(); 
    build(); 
    innovate(); 
}
```

---

## 📅 Date

October 18, 2026

---

## 📄 License

This project is intended for educational and personal use purposes.
