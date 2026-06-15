# 🍔 React Native Meals App

> A restaurant-browsing mobile app built with React Native, Expo, and styled-components.

![React Native](https://img.shields.io/badge/React_Native-0.68-61DAFB?logo=react&logoColor=white)
![Expo](https://img.shields.io/badge/Expo-45-000020?logo=expo&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES2021-F7DF1E?logo=javascript&logoColor=black)
![styled-components](https://img.shields.io/badge/styled--components-5-DB7093?logo=styled-components&logoColor=white)

An early-stage React Native learning project: tab-based mobile UI for a meal-ordering app, with a themed restaurant list, search bar, and bottom-tab navigation. Built on Expo so it runs on iOS, Android, and web from a single codebase.

## ✨ Features

- **Bottom-tab navigation** — Restaurants, Map, and Settings tabs powered by `@react-navigation/bottom-tabs`.
- **Restaurant list screen** — scrollable `FlatList` of restaurant cards rendered with `react-native-paper`.
- **Searchbar UI** — top-of-screen search input ready to be wired up to a real data source.
- **Themed design system** — central `theme` (colors, spacing, fonts) consumed via `styled-components` and a reusable `Spacer` component.
- **Custom Google Fonts** — Oswald and Lato loaded via `expo-font` at startup.
- **Safe-area handling** — `SafeArea` wrapper using `react-native-safe-area-context` so layouts respect notches and status bars.
- **Mocked restaurants service** — promise-based `restaurantsRequest` reads from local mock data, ready to swap for a real API.

> Status: foundation milestone. Map and Settings tabs are placeholder screens — the focus so far is the Restaurants feature, theming, and navigation scaffold.

## 🛠️ Tech Stack

- **Framework** — React Native 0.68 + Expo SDK 45
- **Navigation** — React Navigation v6 (bottom tabs)
- **UI Kit** — `react-native-paper` + `react-native-svg`
- **Styling** — `styled-components/native` with a custom theme
- **Fonts** — `@expo-google-fonts/oswald`, `@expo-google-fonts/lato`
- **Icons** — `@expo/vector-icons` (Ionicons)

## 📁 Project Structure

```
src/
├── components/        # Shared UI primitives (SafeArea, Spacer, Typography)
├── features/
│   └── restaurants/
│       ├── components/    # RestaurantInfoCard + styles
│       └── screens/       # RestaurantsScreen
├── infrastructure/
│   └── theme/         # colors, spacing, fonts, sizes
└── services/
    └── restaurants/   # restaurantsRequest + mock data
```

## 📖 Getting Started

### Prerequisites

- Node.js 16+
- The [Expo Go](https://expo.dev/client) app on your phone (or an iOS/Android simulator)

### Install & run

```bash
# 1. Clone
git clone https://github.com/Vette1123/React-Native-Fully-Interactive-Meals-App.git
cd React-Native-Fully-Interactive-Meals-App

# 2. Install
yarn install            # or: npm install

# 3. Start the Expo dev server
yarn start              # or: npx expo start
```

Then either scan the QR code with Expo Go, press `i` for iOS simulator, or `a` for Android emulator.

### Other scripts

```bash
yarn android    # open on Android
yarn ios        # open on iOS
yarn web        # open in browser via react-native-web
```

## 🙌 Credits

Built by [Mohamed Gado](https://mohamedgado.com) while learning React Native and Expo.
