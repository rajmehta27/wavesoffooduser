# 🍽️ WavesOfFood — Android Food Ordering App

WavesOfFood is a real-time Android-based food ordering system built using **Kotlin**, **Firebase**, and **Razorpay Payment Gateway**.  
It provides a seamless food ordering experience for users and an intuitive management system for restaurant admins — all in real time.

---

## 🎥 Demo Images

<img width="720" height="1600" alt="image" src="https://github.com/user-attachments/assets/657c874f-b0f6-4d30-9f1d-62b667d8fd81" />
<img width="720" height="1600" alt="image" src="https://github.com/user-attachments/assets/d8cde28f-2004-41e8-9684-b81dc35202a2" />
<img width="720" height="1600" alt="image" src="https://github.com/user-attachments/assets/0ebc0ffb-d6a3-41e8-95bf-40af6e00655d" />
![IMG-20251108-WA0028](https://github.com/user-attachments/assets/7056cadc-141b-460d-a884-e7b8da8e1edf)


---

## 🧠 Overview

The application consists of **two interconnected Android apps**:
1. **User App:** Enables customers to browse menus, add items to the cart, make secure payments, and track order status.  
2. **Admin App:** Allows restaurant managers to manage menu items, update order statuses, and synchronize data in real time with the user side.

Built for scalability and simplicity, WavesOfFood merges powerful Firebase services with a modern Kotlin-based Android architecture.

---

## ⚙️ Tech Stack

| Layer | Technology |
|-------|-------------|
| **Frontend** | Kotlin, Android Studio, XML, ViewBinding |
| **Backend (Cloud)** | Firebase Authentication, Firebase Firestore, Firebase Storage |
| **Payments** | Razorpay Android SDK |
| **Design Tools** | Figma, Material Design 3 |
| **Version Control** | GitHub |
| **Testing Tools** | JUnit, Espresso, Firebase Test Lab |

---

## 🚀 Features

### 👨‍🍳 User App
- 🔐 **Secure Authentication** — Firebase Email/Password sign-in  
- 🍔 **Interactive Menu Display** — Real-time menu updates from Firestore  
- 🛒 **Smart Cart System** — Auto total calculation & delivery fee logic  
- 💳 **Razorpay Integration** — Real-money payment simulation via sandbox  
- 📦 **Order Tracking** — Live updates (Pending → Out for Delivery → Delivered)  
- 🔔 **Notifications & History** — Track current and past orders  

### 🧑‍💼 Admin App
- 🥗 **Add & Manage Menu Items** — Add dishes with images via Firebase Storage  
- 📋 **Order Management** — Update and track orders dynamically  
- ⚡ **Real-Time Sync** — Firestore snapshot listeners ensure instant updates  
- 🛠️ **Secure Access** — Admin-only privileges using Firestore rules  

---

## 🏗️ Project Architecture

WavesOfFood/
│
├── user_app/
│ ├── activities/
│ ├── fragments/
│ ├── adapters/
│ ├── models/
│ └── utils/
│
├── admin_app/
│ ├── activities/
│ ├── adapters/
│ ├── models/
│ └── utils/
│
├── media/ (screenshots or videos)
└── README.md

markdown
Copy code

- Both apps share a **common Firebase backend** for real-time updates.
- **Snapshot listeners** ensure live synchronization between users and admins.
- **Razorpay** handles payments securely through encrypted SDK communication.

---

## 🧩 Installation Guide

### 🔹 Prerequisites
- Android Studio (latest version)
- Firebase project configured with Authentication & Firestore
- Razorpay Test Key ID
- Active internet connection

### 🔹 Steps to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/WavesOfFood.git
Open the project in Android Studio.

Connect your Firebase project:

Add google-services.json to app/ folder.

Add your Razorpay Key in the CheckoutActivity.kt file:

kotlin
Copy code
checkout.setKeyID("YOUR_RAZORPAY_KEY_ID")
Build and run the project on an emulator or physical Android device.

🧪 Testing & Debugging
Unit Tests: Implemented using JUnit for logic validation.

UI Tests: Performed with Espresso and manual testing.

Crash Reports: Monitored using Firebase Crashlytics.

Performance Tests: Run via Android Studio Profiler & Firebase Test Lab.

🛠️ Tools & Collaboration
Tool	Purpose
GitHub	Version control and code review
Slack / Discord	Team communication
Google Meet	Weekly review meetings
Figma	UI/UX design and prototyping
Trello	Task tracking and workflow management
Firebase Console	Database and security rule management

👨‍💻 Team Members & Contributions
Name	Role	Contributions
Raj Mehta	Lead Developer & Architect	User App, Razorpay Integration, Firestore Design
Vannsh Agrawal	UI/UX Developer	Layouts, Navigation, and User Experience
Vedika Reddiwar	Backend Developer (Admin App)	Admin logic, Firebase Storage Integration
Chahak Daga	Admin Interface Developer	Admin UI, Order Handling, and Testing

🧭 Challenges Faced
Managing real-time synchronization between User and Admin apps

Handling asynchronous Firestore operations efficiently

Configuring Razorpay SDK callbacks securely

Maintaining consistent UI/UX across multiple Android versions

🏁 Outcome
WavesOfFood successfully delivers a complete, production-grade food ordering system, combining:

Real-time cloud synchronization

Secure online payment integration

Elegant UI design

Scalable Firebase architecture

It demonstrates the team’s ability to conceptualize, design, develop, and deploy a real-world, full-stack Android application.

💡 Future Improvements
🔔 Push notifications via Firebase Cloud Messaging (FCM)

🗺️ Google Maps integration for delivery tracking

🧠 AI-based food recommendations

💬 In-app chat between user and admin

🌙 Dark mode and UI enhancements

📚 References
Android Developer Docs

Firebase Documentation

Razorpay Integration Guide

Material Design Guidelines

Kotlin Language Reference

📄 License
This project is licensed under the MIT License — feel free to use, modify, and enhance it for educational or personal projects.

⭐ Acknowledgements
Special thanks to:

Google Firebase for backend infrastructure

Razorpay for seamless payment integration

Android Developers Community for continuous support and resources

