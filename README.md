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
![image](https://github.com/user-attachments/assets/a81e7a44-2864-433c-b859-513aede03603)
![image](https://github.com/user-attachments/assets/77263423-4f30-48de-b22a-0d07567f3ff2)
![image](https://github.com/user-attachments/assets/b125c091-579f-4d44-8f1f-0456b31e5ec3)
![image](https://github.com/user-attachments/assets/17b9fc5a-e680-4f0f-b35b-757d8b8b8003)
![image](https://github.com/user-attachments/assets/07306d2f-4540-42e7-ab6c-14c450894626)
![image](https://github.com/user-attachments/assets/2e59ae3b-5741-46ef-911e-76eb81b9ed78)
![image](https://github.com/user-attachments/assets/1b492fef-8b2f-4c9c-ab46-ad3960d5252a)
![image](https://github.com/user-attachments/assets/947a094d-5a79-46e5-a701-d9cbb514ec6e)
![image](https://github.com/user-attachments/assets/6fbe579f-75c1-4a60-ba89-486ee0a90964)
![image](https://github.com/user-attachments/assets/2d00ec7c-74bc-4492-99ff-53883786188c)
![image](https://github.com/user-attachments/assets/f3608572-6f85-4051-ab06-582cbc5fedd4)
![image](https://github.com/user-attachments/assets/1da04779-cbc2-4337-a467-c9efa05d4223)












---

## 👩‍💻 Author

**Anju Shaik**  
 
🎓 MS Computer Science  


---

## 📜 License

This project is part of an academic assignment for CSC 392/492 at DePaul University. Educational use only.

