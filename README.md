# FitTrack

FitTrack is a modern, AI-powered fitness tracker Progressive Web App (PWA) built for people who want simple, motivating, and privacy-focused workout tracking.

## ✨ Features

• Intuitive Activity Logging: Add and track workouts, dog walks, and daily activities.
• Beautiful Calendar View: See your workout plans/dates with clear month/day abbreviations.
• Streak Tracking & Progress: Visualize streaks and weekly activity completion.
• Offline-First PWA: Works seamlessly without internet and can be installed like a native app.
• Zero Data Mix/Leak: All user data is stored locally by default—no central server.
• Easy Sharing: Send the app link to others; each user gets their own isolated data vault.
• Automatic Versioning: Every code change is saved and synced to GitHub for full transparency.

## 🚀 Quick Start

1. Install dependencies and run locally:
```
npm install
npm run dev
```

2. Access the app:
Open your browser to the local port (usually http://localhost:5000).

3. Deploy as a PWA:
One-click deploy options and mobile-friendly install for easy testing.

## 📱 How It Works for Users

• Each person using FitTrack via the URL gets their own secure, local data vault.
• Stats, activities, and streaks are completely private (unless shared by the user).
• No analytics/telemetry by default—your fitness data stays with you.

## 🧠 AI & Insights

FitTrack was created to demonstrate how even simple AI-driven summaries and health insights can make daily fitness more motivating and personal. The included models offer gentle feedback, habit reminders, and insight into activity patterns.

## 🛠️ Project Structure

```
fittrack/
  ├── client/           # Frontend code (React/TS)
  ├── server/           # Backend code for API/extensions (optional)
  ├── shared/           # Shared types/interfaces
  ├── components.json   # UI and feature registry
  ├── drizzle.config.ts # Database config (PostgreSQL or SQLite)
  ├── package.json      # Project metadata and scripts
  └── README.md         # This file
```

## ⚙️ Configuration

• IndexedDB: Handles default local data storage.
• Replit Auth (optional): For experiments with user login/profiles.
• PostgreSQL (optional): Enable for cloud sync or multi-user (see notes below).

## 🔒 Privacy by Design

• No user accounts or data sharing unless explicitly enabled.
• Each device/browser instance is independent, ensuring users' fitness data is theirs alone.

## 📊 Analytics

• Google Analytics integration is available but optional.
To enable, set your VITE_GA_MEASUREMENT_ID environment variable.

## 🧑‍💻 Multi-User & Sync Notes

To support true multi-user accounts, live sync, and cross-device dashboards:

• Enable authentication + PostgreSQL backend.
• Update data models to associate all records with user IDs.
• Implement cloud/local sync patterns.

See the roadmap in issues for details!

## 🙌 Contributing

1. Fork this repo or open issues for features/bugs.
2. All commits auto-versioned and pushed to GitHub.
3. Pull requests are welcome!

## 📄 License

MIT License. See LICENSE file for details.
