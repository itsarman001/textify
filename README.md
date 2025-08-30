# 🌐 Chrome New Tab - Vue.js Extension

A customizable **Chrome New Tab** page built with **Vue.js**. This extension transforms your new tab into a powerful dashboard with:

- 🔖 Real-time bookmark sync with Chrome
- ✅ A lightweight to-do list
- 📆 Google Calendar integration
- 🔍 Multi-provider search bar
- 🌤️ Weather forecast
- 🕒 Live time display

---

## 📸 Preview

_(Add a screenshot or demo GIF here)_

---

## 🚀 Features

| Feature                | Description                                         |
| ---------------------- | --------------------------------------------------- |
| 🔖 **Bookmarks**       | Sync with Chrome Bookmarks API (read/create/delete) |
| ✅ **To-Do List**      | Manage daily tasks using local or Chrome storage    |
| 📆 **Google Calendar** | Show upcoming events with OAuth-based sync          |
| 🔍 **Search Bar**      | Switch between Google, DuckDuckGo, Bing, etc.       |
| 🌤️ **Weather**         | Fetch forecast using OpenWeather or WeatherAPI      |
| 🕒 **Time**            | Real-time clock with date                           |

---

## 🧱 Tech Stack

- [Vue 3](https://vuejs.org/)
- [Vite](https://vitejs.dev/)
- Chrome Extension Manifest V3
- Google Calendar API
- OpenWeatherMap API
- Chrome Bookmarks & Storage APIs

---

## 📁 Project Structure

```bash
src/
├── components/
│   ├── Bookmark/
│   ├── Todo/
│   ├── Calendar/
│   ├── Search/
│   ├── Weather/
│   └── Time/
├── composables/
├── services/
├── views/
└── App.vue
```

---

## 🔧 Setup & Development

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/chrome-new-tab.git
cd chrome-new-tab
```

### 2. Install Dependencies

```bash
pnpm install
```

### 3. Start Dev Server

```bash
pnpm dev
```

> This runs the app in development mode. Use something like [Extension Reloader](https://chrome.google.com/webstore/detail/extension-reloader) to reload your extension quickly while developing.

---

## 🧪 Build for Production

```bash
pnpm build
```

Then load the `dist/` folder as an **Unpacked Extension** in Chrome:

1. Open `chrome://extensions/`
2. Enable **Developer Mode**
3. Click **Load unpacked** and select the `dist/` folder

---

## 🔐 Environment Variables

Create a `.env` file:

```env
VITE_GOOGLE_API_KEY=your_api_key
VITE_GOOGLE_CLIENT_ID=your_client_id
VITE_WEATHER_API_KEY=your_weather_api_key
```

---

## 🗃️ Chrome Permissions Required

```json
"permissions": [
  "bookmarks",
  "storage",
  "identity",
  "tabs"
]
```

---

## 📅 Roadmap

- [x] Chrome bookmark two-way sync
- [x] To-do card with local persistence
- [x] Google Calendar event integration
- [x] Weather + time components
- [ ] Custom theme support
- [ ] Responsive layout improvements

---

## 📄 License

MIT License

---

## 🙌 Credits

Built with ❤️ using Vue and Vite by \[Md Arman]

> Inspired by productivity dashboards like Momentum and custom new tab experiences.
