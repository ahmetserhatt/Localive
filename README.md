
# 📱 LocaLive – Location-Based Event Planning App

## 🔍 Overview
**LocaLive** is a full-stack mobile application that allows users to discover, manage, and plan events based on their current location. It provides automatic and manual location tracking, ticket recommendations, and an interactive map interface.

> 🎫 **Event data is retrieved from the [Ticketmaster API](https://developer.ticketmaster.com/)** and enhanced with **AI-based personalized recommendations** for a more tailored user experience.

---

## 🧩 Project Structure

```
LocaLive/
├── LocaLive-Frontend/   # Kotlin-based Android app
└── LocaLive-Backend/    # ASP.NET Core Web API
```

---

## 💡 Key Features

| Layer      | Highlights |
|------------|------------|
| **Frontend** | Kotlin + Android SDK, Retrofit, MVVM-ish structure, WebView for interactive map display, Fused Location Provider for GPS |
| **Backend** | ASP.NET Core, Entity Framework, REST API, layered architecture |
| **AI Integration** | Suggests events using ML logic (based on preferences & Ticketmaster data) |
| **Data Source** | Ticketmaster API (live concerts, festivals, exhibitions, etc.) |

---

## 🛠 Tech Stack

| Frontend (Mobile) | Backend (API) |
|-------------------|----------------|
| Kotlin            | ASP.NET Core   |
| Retrofit          | Entity Framework |
| WebView + JS      | LINQ / C#      |
| Location Services | REST API       |

---

## 🚀 Setup Instructions

### Backend Setup

```bash
cd LocaLive-Backend/LocaLive
dotnet restore
dotnet run
```

- Make sure to configure `appsettings.json` for your database and CORS setup.

### Frontend Setup

- Open `LocaLive-Frontend/LocaLive` in **Android Studio**
- Build and run on emulator or real device
- Update `baseUrl` inside `ApiClient.kt` to match your local IP (e.g., `10.0.2.2` for emulator)

---

## 🧠 AI Recommendations

LocaLive uses rule-based or lightweight ML logic to:
- Rank upcoming events based on location, preferences, and history
- Suggest relevant experiences (e.g., concerts, exhibitions, local fests)

---

## 📸 Screenshots

- Login / Signup screens
- Location selection & GPS auto-detect
- AI-recommended events
- Interactive map with event markers
- Ticket links and plan suggestions

---

## 🤝 Contributing

We welcome pull requests, ideas, and contributions. Please target the `develop` branch.

---

## 📄 License

MIT License. See `LICENSE` file for details.
