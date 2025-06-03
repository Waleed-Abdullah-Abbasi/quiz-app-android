![image](https://github.com/user-attachments/assets/877c6066-0fc5-4d42-ac64-bf2f404e4b0c)


## 📱 Quiz App - Android Application

[![Android](https://img.shields.io/badge/Platform-Android-green.svg)](https://developer.android.com)
[![Firebase](https://img.shields.io/badge/Backend-Firebase-orange.svg)](https://firebase.google.com)
[![Material Design](https://img.shields.io/badge/Design-Material%20Design%203-blue.svg)](https://material.io)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A modern Android Quiz Application built with Firebase Authentication, Material Design 3, and clean architecture principles. This repository contains Part-1 implementation focusing on user authentication and app foundation.

## 🚀 Features

### 🔐 Authentication System
- **Firebase Email/Password Authentication**
- **Secure User Session Management**
- **Password Recovery via Email**
- **Input Validation & Error Handling**
- **Google Sign-In Ready** (Part-2)

### 🎨 Modern UI/UX
- **Material Design 3 Components**
- **Animated Splash Screen**
- **Responsive Layouts**
- **Loading States & Progress Indicators**
- **Custom Styled Components**

### 🏗️ Architecture
- **Clean Activity Structure**
- **Firebase Integration**
- **Modular Design Pattern**
- **Error Handling Framework**

## 📱 Screenshots

| Splash Screen | Login Screen | Home Screen |
|---------------|--------------|-------------|
| ![Splash](screenshots/splash.png) | ![Login](screenshots/login.png) | ![Home](screenshots/home.png) |

## 🛠️ Tech Stack

- **Language**: Java
- **IDE**: Android Studio
- **Backend**: Firebase Authentication
- **UI Framework**: Material Design 3
- **Layout**: ConstraintLayout
- **Animation**: Android Animation Framework
- **Validation**: Android Patterns & TextUtils

## 📋 Prerequisites

Before running this project, make sure you have:

- Android Studio (Latest Version)
- Java Development Kit (JDK 8 or higher)
- Android SDK (API Level 21+)
- Firebase Account
- Google Services JSON file

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/quiz-app-android.git
cd quiz-app-android
```

### 2. Firebase Configuration
1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create a new project or select existing one
3. Add Android app with your package name
4. Download `google-services.json`
5. Place the file in `app/` directory
6. Enable Authentication → Email/Password in Firebase Console

### 3. Open in Android Studio
1. Open Android Studio
2. Click "Open an existing project"
3. Navigate to the cloned directory
4. Wait for Gradle sync to complete

### 4. Update Package Name
1. Update package name in `AndroidManifest.xml`
2. Update package name in all Java files
3. Update `applicationId` in `app/build.gradle`

### 5. Run the Application
1. Connect Android device or start emulator
2. Click "Run" button in Android Studio
3. App will install and launch automatically

## 📁 Project Structure

```
app/
├── src/main/
│   ├── java/com/yourpackage/quizapp/
│   │   ├── SplashActivity.java          # Entry point with auth check
│   │   ├── LoginActivity.java           # Authentication interface
│   │   ├── HomeActivity.java            # Main dashboard
│   │   └── ForgotPasswordActivity.java  # Password recovery
│   ├── res/
│   │   ├── layout/                      # XML layout files
│   │   ├── drawable/                    # Custom drawables & backgrounds
│   │   ├── values/                      # Colors, strings, styles
│   │   └── anim/                        # Animation resources
│   └── AndroidManifest.xml
├── build.gradle (Module: app)
└── build.gradle (Project)
```

## 🔄 App Flow

```
SplashActivity (3s animation)
    ↓
Authentication Check
    ↓                    ↓
✅ Logged In        ❌ Not Logged In
    ↓                    ↓
HomeActivity        LoginActivity
    ↓                    ↓
Logout Button    Login/Forgot Password
    ↓                    ↓
LoginActivity     HomeActivity/Reset
```

## 🧪 Testing

### Manual Testing Checklist
- [ ] Splash screen displays for 3 seconds
- [ ] Login with valid credentials works
- [ ] Login with invalid credentials shows error
- [ ] Email validation works correctly
- [ ] Password validation (min 6 chars) works
- [ ] Forgot password sends reset email
- [ ] Home screen shows user email
- [ ] Logout functionality works
- [ ] App remembers login state

### Test Credentials
For testing purposes, create a test account in Firebase Console or use the app's registration flow when implemented in Part-2.

## 🔮 Roadmap (Upcoming Features)

### Part-2 Implementation
- [ ] **Google Sign-In Integration**
- [ ] **User Registration System**
- [ ] **Quiz Question Interface**
- [ ] **Score Tracking System**
- [ ] **Results & Analytics**
- [ ] **Multiple Quiz Categories**
- [ ] **Leaderboard System**
- [ ] **Offline Mode Support**

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Coding Standards
- Follow Java naming conventions
- Add comments for complex logic
- Maintain consistent indentation
- Update documentation for new features
