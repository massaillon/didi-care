# 💙 Didi Care – Divine's Diabetes Companion

**Developed with love by Massaillon Silué**

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Android](https://img.shields.io/badge/Android-14-green.svg)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-2.0-purple.svg)](https://kotlinlang.org)

## 🏥 Overview

**Didi Care** is a **native Android** application (Kotlin + Jetpack Compose) designed to empower Divine Eberechukwu Bernard, a 28-year-old teacher with Type 1 Diabetes, to take control of her health with grace, culture, and love.

### Quick Stats
- **Platform:** Native Android (Kotlin + Jetpack Compose)
- **Version:** 2.0 Enhanced
- **Min SDK:** 29 (Android 10)
- **Target SDK:** 34 (Android 14)
- **Package Name:** `com.massillon.didicare`
- **User:** Eberechukwu Divine Bernard (28, Type 1 Diabetes)
- **Medication:** Novomix 30/70 (18u AM / 16u PM)
- **Location:** Abidjan, Côte d'Ivoire
- **Support System:** Philippe (boyfriend, view-only access)

---

## 🎯 Vision

> "To make Divine feel in control, encouraged, and culturally understood—transforming daily diabetes tasks from burdensome to beautiful, with restaurant-quality meals, home cycling, outdoor walking with GPS tracking, and AI-powered insights that match her professional identity."

---

## 🎨 Design Philosophy

- **Aesthetic:** Pastel girly (lavender #E6E6FA → peach #FFDAB9 → mint #98FF98 → soft pink #FFB6C1)
- **Typography:** Rounded corners (16–20dp), Poppins/Nunito fonts
- **Animations:** Fluid, heart symbols ✨💙
- **Culinary Heritage:** 300 professional West African & North African dishes (5-star restaurant quality names)
- **Offline-First:** Real-time cloud sync via Firebase
- **Accessibility:** Voice commands, TTS feedback, Wear OS support

---

## 📱 Features (13 Screens)

### Core Screens
1. **Splash & Onboarding** – Welcome Divine with voice greeting
2. **Home Dashboard** – Personalized greeting, next insulin countdown, quick actions
3. **Insulin Logging** – Novomix pen tracker with injection site rotator + correction dose calculator
4. **Blood Glucose Entry** – BG logger with 7-day trend graph + CGM integration
5. **"Mama's Pot"** – 300-dish meal planner (all professional names, diabetes-safe)
6. **Physical Activity Tracker** – Home Cycling 🚴‍♀️ (indoor) + Walking 🚶‍♀️ (GPS + location sharing)
7. **Medical Records Vault** – PDF upload & OCR extraction
8. **Doctor Profile & Appointments** – Telehealth video calls
9. **Sleep & Stress Logger** – Daily tracking + correlation insights
10. **SOS Hypo Button** – Emergency SMS + GPS to Philippe
11. **AI Health Insights** – Correlations, predictions, personalized recommendations
12. **Community** – "Didi Sisters" support forum (moderated)
13. **Profile & Rewards** – Gamification (badges, points, streaks)

---

## 🏃 Activity Tracking

### 🚴‍♀️ Home Cycling (Indoor, No GPS)
- ✅ NO location tracking (stationary bike)
- ✅ Distance estimation from cadence × time
- ✅ Heart rate monitoring (optional Bluetooth HR monitor)
- ✅ Resistance level tracking (1–10)
- ✅ Motivation message from Philippe
- ✅ Post-cycling BG prediction

### 🚶‍♀️ Walking (Outdoor, GPS + Location Sharing)
- ✅ Real-time GPS map (Google Maps, blue dot + green polyline)
- ✅ Share location via WhatsApp/SMS/Telegram/Email
- ✅ Live location sharing to Philippe (every 10 min, optional)
- ✅ Distance: GPS-measured (accurate ±5%)
- ✅ Steps tracking (Android StepDetector)
- ✅ Pace calculation (min/km)
- ✅ Post-walking BG prediction

### ⚠️ Safety Features
- **Interlock:** Can't run both simultaneously
- **BG Guard:** Blocks if BG <100 mg/dL or >250 mg/dL
- **Predictive Alerts:** Warns of hypo/hyper risk in 30–60 min

---

## 🍽️ "Mama's Pot" – 300 Professional Dishes

All dishes are:
- **Diabetes-Safe:** Low glycemic index (GI <50)
- **High-Protein:** 15–30g protein per serving
- **Professional Names:** 5-star restaurant quality
- **Culturally Authentic:** West African & North African recipes

---

## 🤖 AI Health Insights

- **Correlations:** "On days you cycle >20 min, evening BG drops 15% on average"
- **Predictive Alerts:** "Hypo risk in 45 min (85%). Eat 15g carbs now."
- **Sleep Analysis:** "Sleep <7 hours → morning BG 20% higher"
- **Stress Detection:** "Stressful days: BG averages 50 mg/dL higher"

---

## 🗄️ Database (ROOM + SQLCipher)

All data encrypted with **SQLCipher (AES-256)**.

```
⦿ insulin_logs
⦿ bg_readings
⦿ physical_activities
⦿ meal_diary
⦿ carbs_database
⦿ pdf_records
⦿ doctor_profiles
⦿ sleep_stress
⦿ ai_insights
⦿ predictions
⦿ achievements
⦿ shared_locations
��� cgm_readings
⦿ voice_commands
```

---

## ☁️ Cloud Sync (Firebase)

- **Firestore:** Real-time sync
- **Storage:** PDF records
- **Auth:** Email/password + biometric
- **Messaging (FCM):** Push notifications

---

## 🔒 Security & Privacy

- **SQLCipher:** AES-256 encryption
- **Firebase Auth:** Secure authentication
- **HTTPS/TLS 1.3:** All network traffic encrypted
- **GDPR Compliant:** Data export & deletion
- **On-Device ML:** TensorFlow Lite (privacy-first)

---

## 🚀 Getting Started

### Prerequisites
- Android Studio Hedgehog (2023.1.1) or later
- JDK 17+
- Android SDK 34 (Android 14)
- Gradle 8.0+

### Clone Repository
```bash
git clone https://github.com/massaillon/didi-care.git
cd didi-care
```

### Build & Run
```bash
./gradlew clean
./gradlew assembleDebug
./gradlew installDebug
```

---

## 📄 License

MIT License – See [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Developer

**Massaillon Silué**

Developed with love by Massaillon Silué 💙

For Divine Eberechukwu Bernard – Teacher, Warrior, Beloved.

---

**Didi Care 💙** – *Making diabetes management beautiful, one day at a time.*
