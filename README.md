# 🚍 CTA Bus Tracker App

A mobile application developed for Android using the CTA Bus Tracker API that allows users to view real-time route, stop, and prediction information for CTA buses in Chicago. This project was created as part of the CSC 392/492 course at DePaul University.

---

## 📱 Features

- 📍 **Nearby Stops**: Shows bus stops within 1000 meters of the user's location.
- 🔍 **Search Routes**: Easily find routes by number or name.
- 🔁 **Direction-Based Stops**: View bus stops based on selected route and direction.
- 🕑 **Live Predictions**: Displays real-time bus arrival times and vehicle distances.
- 🔄 **Swipe to Refresh**: Pull down in the predictions screen to refresh data.
- 🎨 **Polished UI**: Implements Google’s Splash Screen API and custom fonts for a modern feel.
- 📢 **Ad Support**: Integrates banner ads (using AdMob or Unity).
- 💾 **Smart Caching**: Routes and stops cached for 24 hours to minimize API calls.

---

## 🧱 App Structure

### Activities

- **MainActivity**: Displays all CTA routes and allows search.
- **StopsActivity**: Shows relevant stops based on route and direction, filtered by proximity.
- **PredictionsActivity**: Shows live prediction info for a selected stop.

---

## 🛠️ Technologies Used

- **Language**: Java
- **Platform**: Android
- **API**: [CTA Bus Tracker API](https://www.transitchicago.com/developers/bustracker/)
- **Libraries & Features**:
  - Location Services
  - AlertDialogs
  - TextInputLayout
  - Custom Fonts
  - Banner Ads (AdMob/Unity)
  - Google’s SplashScreen API

---

## 🔐 Permissions

- Requests **location permission** at runtime.
- If denied twice, a rationale dialog explains the reason.
- If denied again, the app exits gracefully.

---

## 🔌 API Integration

The following CTA Bus Tracker API endpoints are used:

- `getroutes` – Lists all CTA routes.
- `getdirections` – Provides directions for a selected route.
- `getstops` – Fetches stops for a route/direction combo.
- `getpredictions` – Retrieves upcoming buses for a specific stop.

> **Note**: Replace `"your API key here"` wherever needed in the code.

---

## 🗂 Directory Overview

```
├── MainActivity.java
├── StopsActivity.java
├── PredictionsActivity.java
├── utils/
│   ├── ApiManager.java
│   └── CacheUtils.java
├── assets/
│   └── helvetica_neue_medium.ttf
└── res/
    ├── layout/
    └── values/
```

---

## 🧩 Caching

- Route and stop data is cached for **24 hours**.
- Predictions are **not cached** to ensure real-time accuracy.

---

## 🧪 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/shaikanju/CTA-BUS-Tracker-APP.git
   ```
2. Open the project in **Android Studio**.
3. Replace any placeholder `"your API key here"` with your actual **CTA API Key**.
4. Add your **AdMob or Unity ad unit IDs** to each activity.
5. Enable location permissions on your device or emulator.
6. Build and run!

---

## 📷 Screenshots
![image](https://github.com/user-attachments/assets/4954595d-1d89-4342-a6fa-526681d76980)
![image](https://github.com/user-attachments/assets/1b0b9a85-05af-462f-876c-94c976822018)
![image](https://github.com/user-attachments/assets/4e7b1a0a-8d79-41c4-ad2d-f5c4b87a2dd4)
![image](https://github.com/user-attachments/assets/9f1b6ef8-e267-49f8-94cb-d0c9611e7c6f)
![image](https://github.com/user-attachments/assets/7f0497e2-1b0f-4a0d-9eaf-3dc4c6b61868)
![image](https://github.com/user-attachments/assets/4ec8362b-a220-40e7-b3e4-d703485a36ec)
![image](https://github.com/user-attachments/assets/d7979309-bd6f-4f16-9eed-6de96d5d6e2e)
![image](https://github.com/user-attachments/assets/e033383d-55ae-4914-b6c0-eb03f50d6cbb)
![image](https://github.com/user-attachments/assets/6ee49204-8ed2-483e-99a4-bab7174e2683)
![image](https://github.com/user-attachments/assets/b0bad444-ffc1-4c1b-a575-27878050ac88)
![image](https://github.com/user-attachments/assets/20b70b7f-b465-473d-8a94-97598ade7cd7)

---

## 👩‍💻 Author

**Anju Shaik**  
 
🎓 MS Computer Science  


---

## 📜 License

This project is part of an academic assignment for CSC 392/492 at DePaul University. Educational use only.

