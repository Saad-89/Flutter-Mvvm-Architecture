# 📱 Flutter MVVM Architecture Template

Welcome to the Flutter MVVM Architecture Template!  
This repository demonstrates a clean and scalable way to structure a Flutter app using the **MVVM (Model-View-ViewModel)** pattern. It's designed to help developers maintain separation of concerns, write testable code, and scale applications efficiently.

---

## 🧠 What is MVVM?

**MVVM (Model-View-ViewModel)** is an architectural pattern that separates concerns into three main components:

- **Model**: Manages the data, business logic, and backend interactions (like APIs or databases).
- **View**: The UI that displays data and reacts to changes.
- **ViewModel**: The bridge between the Model and the View. It processes logic, updates UI state, and exposes it for the View to consume.

### 🔄 How It Works:
1. The user interacts with the **View**.
2. The **ViewModel** processes the action and updates the relevant state.
3. The **Model** fetches or updates data as needed.
4. The **ViewModel** updates the state.
5. The **View** listens to state changes and rebuilds accordingly.

---

## 📁 Project Structure

```text
lib/
├── core/           # Common utilities, constants, themes, extensions
├── data/           # API, repository, and local database logic
│   └── models/     # Data models used throughout the app
├── view/           # All UI components
│   └── screens/    # Each screen folder with related widgets
├── viewmodel/      # ViewModels managing state and business logic
├── services/       # App services like Auth, API, SharedPreferences
├── routes/         # App navigation and route management
└── main.dart       # App entry point
