# 🥗 NutriLife Pro

> **A modern, interactive nutrition and wellness dashboard built with HTML, CSS and JavaScript.**

NutriLife Pro is a client-side nutrition platform that brings everyday health-planning tools into one responsive web application. It combines calorie and macro tracking with BMI/BMR calculations, diet planning, recipe creation, meal preparation, food search, progress visualisation, and browser-based data persistence.

## ✨ Features

- 🧮 **Nutrition Calculator** — track calories, protein, carbohydrates, fat, fibre and sugar for foods added to the daily log.
- 🔥 **BMR & TDEE Calculator** — estimate basal metabolic rate and daily energy requirements from user inputs.
- 📏 **BMI Calculator** — calculate BMI and display a corresponding health category and guidance.
- 🍽️ **Diet Plan Generator** — generate meal plans based on goals, preferences and meal frequency.
- 👨‍🍳 **Recipe Maker** — create, save and delete custom recipes with ingredients and nutrition information.
- 🗓️ **Meal Prep Planner** — organise selected recipes into a multi-day meal-prep schedule and shopping list.
- 🔎 **Food Database** — search, filter and sort a built-in nutrition database.
- 📊 **Progress Dashboard** — visualise nutrition and weight information using Chart.js.
- 💾 **Local Storage** — keep recipes, diet plans, weight entries, goals and daily food data in the browser.
- 📱 **Responsive UI** — desktop and mobile navigation with a dark, modern dashboard design.

## 🖥️ Preview

> Add screenshots or a short GIF here after publishing the project.

| Dashboard | Nutrition Tools |
|---|---|
| `screenshots/dashboard.png` | `screenshots/calculators.png` |

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5** | Application structure and semantic content |
| **CSS3** | Custom styling, animations and responsive presentation |
| **JavaScript (ES6+)** | Calculations, UI interactions, data handling and application logic |
| **Tailwind CSS CDN** | Utility-first layout and styling |
| **Chart.js** | Progress and nutrition charts |
| **Font Awesome** | Interface icons |
| **Web LocalStorage API** | Client-side persistence |

## 🧠 How It Works

```text
                ┌─────────────────────┐
                │   User Information  │
                │ age / height / etc. │
                └──────────┬──────────┘
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
        ┌──────────┐  ┌──────────┐  ┌──────────┐
        │   BMR    │  │   BMI    │  │ Nutrition│
        │ Calculator│ │ Calculator│ │  Tracker │
        └────┬─────┘  └──────────┘  └────┬─────┘
             │                            │
             ▼                            ▼
        ┌──────────┐                ┌────────────┐
        │   TDEE   │                │ Food Data  │
        │ & Goals  │                │  Database  │
        └────┬─────┘                └─────┬──────┘
             │                            │
             └─────────────┬──────────────┘
                           ▼
                  ┌─────────────────┐
                  │ Diet / Meal Plan│
                  │ Recipe / Progress│
                  └────────┬────────┘
                           ▼
                    Browser Storage
```

## 📂 Project Structure

```text
nutrilife-pro/
│
├── index.html          # Main application interface
├── styles.css          # Custom CSS and animations
├── script.js           # Nutrition logic and UI interactions
├── README.md           # Project documentation
├── .gitignore          # Git exclusion rules
└── screenshots/        # Optional project screenshots
```

## 🚀 Run Locally

No backend or build system is required.

### Option 1 — Open directly

1. Clone the repository.
2. Open `index.html` in a modern browser.

### Option 2 — VS Code Live Server

1. Clone the repository.
2. Open the folder in VS Code.
3. Install the **Live Server** extension if needed.
4. Right-click `index.html` → **Open with Live Server**.

The application loads its UI libraries from CDNs, so an internet connection is recommended.

## 📊 Main Calculations

### BMR

The application uses the **Mifflin–St Jeor equation** to estimate Basal Metabolic Rate from age, sex, height and weight, then uses activity level to estimate daily energy requirements.

### BMI

BMI is calculated from body weight and height and mapped to a standard category for the application's guidance display.

> **Note:** NutriLife Pro is an educational/project application and is not a substitute for professional medical or dietary advice.

## 💾 Data & Privacy

NutriLife Pro is a front-end application. User-created recipes, diet plans, food logs, goals and weight entries are stored locally using the browser's `localStorage` API. No custom backend or account system is included in the current version.

## 🔮 Future Improvements

- [ ] Add a backend and user authentication
- [ ] Sync data across devices
- [ ] Add downloadable nutrition reports
- [ ] Add more regional foods and serving-size options
- [ ] Add a public nutrition API integration
- [ ] Add accessibility improvements and automated UI testing
- [ ] Deploy a production version with a custom domain

## 👨‍💻 Author

**Samarth Shinde**

Built as a web development / nutrition technology project.

## 📄 License

This project is available under the MIT License. See `LICENSE` for details.
