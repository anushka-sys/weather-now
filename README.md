# 🌦️ Weather Now — React Weather App

**Weather Now** is a simple and elegant weather app built for **Jamie**, an outdoor enthusiast who wants to quickly check the current weather conditions for any city in the world.  

The app fetches real-time weather data using the **Open-Meteo API** and presents it in a clean, responsive interface.

---

## Live Deployed Link
https://weathercheker.netlify.app/


---
## 📸 Project images  

<img width="800" height="640" alt="image" src="https://github.com/user-attachments/assets/b9a9d307-2895-4d14-b8ab-0fb672531c29" />

  ### Light Mode

<img width="800" height="640" alt="image" src="https://github.com/user-attachments/assets/5e92324c-a0d5-42bf-9376-1fa1faafc2dc" />

## 🚀 Features

### 🌤 Core Features
- Search weather by **city name**  
- View **temperature**, **wind speed**, and **humidity**  
- See **current weather condition** (sunny, cloudy, rainy, etc.)  
- Responsive and works smoothly on both **desktop and mobile**

### 💡 Supporting Features
- Displays **"feels like" temperature**
- Shows **weather icons** for conditions (e.g., sun, clouds, rain)
- Displays **last updated time**
- Friendly **loading** and **error** states

### 🌈 Optional Enhancements (Future Ideas)
- Auto-detect current location  
- Dark/Light mode toggle  
- Save recent searches  
- 5-day forecast extension  

---

## 🎨 UI/UX Design

- **Color palette:** Calm black & whites for a fresh outdoor look  
- **Layout:**
  - Search bar at the top  
  - Main weather card in the center  
  - Additional info (humidity, wind, feels like) below  
- **Responsive design** using **Tailwind CSS**
- **Weather icons** via [Lucide Icons](https://lucide.dev/) or [React Icons](https://react-icons.github.io/react-icons/)

---

## ⚙️ Tech Stack

- **Frontend:** React.js (with Hooks)
- **Styling:** Tailwind CSS
- **API:** [Open-Meteo API](https://open-meteo.com/)
- **Icons:** React Icons / Lucide React

---

```bash
weather-app/
|
|-- index.html
|-- package.json
|-- tsconfig.json
|-- vite.config.ts
|
|-- src/
|   |-- api/
|   |   |-- types.ts
|   |   |-- weather.ts              # Handles all Open-Meteo API calls
|   |
|   |-- hooks/
|   |   |-- use-weather.ts          # Fetches weather data using React Query
|   |   |-- use-geolocation.ts      # Gets user's current location
|   |   |-- use-favorite.ts         # Manages favorite cities
|   |   |-- use-local-storage.ts    # Wrapper for localStorage
|   |   |-- use-search-history.ts   # Keeps track of recent searches
|   |
|   |-- components/
|   |   |-- layout.tsx
|   |   |-- header.tsx
|   |   |-- city-search.tsx
|   |   |-- current-weather.tsx
|   |   |-- weather-details.tsx
|   |   |-- weather-forecast.tsx
|   |   |-- hourly-temprature.tsx
|   |   |-- loading-skeleton.tsx
|   |   |-- favorite-button.tsx
|   |   |-- favorite-cities.tsx
|   |   |-- theme-toggle.tsx
|   |   |
|   |   |-- ui/
|   |       |-- alert.tsx
|   |       |-- button.tsx
|   |       |-- card.tsx
|   |       |-- dialog.tsx
|   |       |-- skeleton.tsx
|   |       |-- tooltip.tsx
|   |    
|   |
|   |-- context/
|   |   |-- theme-provider.tsx      # Manages light/dark theme
|   |
|   |-- lib/
|   |   |-- utils.ts                # Helper functions
|   |
|   |-- pages/
|   |   |-- weather-dashboard.tsx   # Main dashboard - combines all features
|   |   |-- city-page.tsx           # Detailed view for a selected city
|   |
|   |-- App.tsx                     # App entry - routing, theme, and query setup
|   |-- main.tsx                    # Renders root React app
|   |-- index.css                   # Global styling
|
`-- README.md

```


### 🔁 Data Flow

1. Jamie types a city name in the **SearchBar**
2. The app fetches **latitude & longitude** (optional if needed)
3. Calls **Open-Meteo API** for real-time weather data
4. Displays data in **WeatherCard**
5. Shows **Loading** state during fetch and **ErrorMessage** if request fails

---

## 🧠 Thought Process

This project was designed with **user empathy** — keeping Jamie’s needs first:
- Focused on **speed and clarity** — quick access to weather info
- Simple **one-screen design** to avoid clutter
- **Error handling** for invalid cities or API issues
- Responsive layout for outdoor use on mobile devices

---

## 🔍 API Reference (Open-Meteo)

Example API call:

https://api.open-meteo.com/v1/forecast?latitude=51.5072&longitude=0.1276&current_weather=true




You can use the [Geocoding API](https://open-meteo.com/en/docs/geocoding-api) to fetch coordinates by city name if needed.



## 💬 Error & Loading States

- **Loading:** Shows spinner with “Fetching weather data…” message  
- **Error:** Shows friendly message like “City not found. Try again!”  
- **Network error:** “Unable to reach weather service. Please check your connection.”

---

## 🧪 Testing Checklist

✅ Enter valid city → correct weather info displayed  
✅ Invalid city → error message shown  
✅ Loading spinner appears during fetch  
✅ Layout adapts to mobile screen  
✅ Weather icons update correctly based on conditions  

---

## ✨ Final Touches

- Smooth fade-in animation on weather card  
- Subtle hover effect on search button  
- Friendly empty state (e.g., “Search for a city to see the weather”)  
- Modern and clean typography using Tailwind defaults  

---

## 🧑‍💻 Author

👩‍💻 **Anushka Wabale**  
🌐 GitHub: [@anushka-sys](https://github.com/anushka-sys)  
🔗 LinkedIn: [Anushka Wabale](https://www.linkedin.com/in/anushka-wabale/)  
🐦 X (Twitter): [@anushka_sys](https://x.com/anushka_sys)  

