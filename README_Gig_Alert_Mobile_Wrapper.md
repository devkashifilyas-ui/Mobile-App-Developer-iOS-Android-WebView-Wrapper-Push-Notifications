
# Gig Alert Mobile Wrapper (iOS + Android)

Production-ready Flutter WebView wrapper with reliable real-time push notifications and deep linking.

---

## 🚀 Project Overview

This mobile application wraps an existing React web platform inside a secure WebView and delivers real-time gig alert push notifications using Firebase Cloud Messaging (FCM).

Designed for:
- High-volume notification delivery
- Low-cost infrastructure (FCM = Free)
- Deep linking into specific pages
- Full App Store & Google Play approval readiness
- 1 month post-launch support

---

## 🧱 Architecture

Azure (.NET Backend)
        ↓
Firebase Cloud Messaging (FCM)
        ↓
Android + iOS Devices
        ↓
Deep Link Handler
        ↓
Secure WebView → React Web App

---

## 🛠 Tech Stack

- Flutter (single codebase)
- Firebase Cloud Messaging
- Native WebView (hardened)
- Deep Linking (Universal Links + Android Intent Filters)
- Azure backend integration (.NET compatible)
- Optional: Firebase Crashlytics for monitoring

---

## 🔔 Push Notification Flow

1. User logs in
2. App generates FCM token
3. Token stored in Azure backend
4. Backend sends push via FCM HTTP v1
5. Notification includes deep_link payload
6. App opens correct page inside WebView

---

## 📦 Folder Structure

lib/
 ├── main.dart
 ├── services/
 │    ├── notification_service.dart
 │    ├── deep_link_service.dart
 ├── screens/
 │    ├── webview_screen.dart
 ├── config/
 │    ├── constants.dart

android/
ios/

---

## 📲 Features

- Secure WebView wrapper
- Real-time push notifications
- Background + killed-state support
- Deep linking
- Store compliance hardened
- Production-ready deployment structure

---

## 🧪 Testing Matrix

- Foreground notifications
- Background notifications
- App terminated state
- Deep link cold start
- Network failure handling
- Session expiration handling

---

## 📈 Scalability & Cost

Push Notifications: Free via FCM  
No third-party push providers required  
Scales to millions of users  

---

## 🏁 Deployment Steps

1. Add Firebase config files (GoogleService-Info.plist & google-services.json)
2. Configure bundle IDs
3. Enable Push Capabilities (iOS)
4. Setup universal links
5. Generate TestFlight build
6. Upload to Google Play Internal Testing
7. Submit for store review

---

## 💼 Milestone Plan

1️⃣ Architecture + WebView + Deep Linking – $1,200  
2️⃣ Push System + Hardening – $1,200  
3️⃣ Store Deployment – $1,000  
4️⃣ 1 Month Post Launch Support – $600  

Ongoing support: USD 20/hour

