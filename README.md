# News App

News App is an Android application built with Jetpack Compose and follows a clean architecture pattern. It fetches news articles from NewsAPI, allowing users to read top headlines, save favorites, and search articles.

---

## Features

Top Headlines: Access the latest news from various categories.
Favorites: Save articles locally for offline reading.
Search Functionality: Find news articles using keywords.
Error Handling: Handles network and API errors gracefully.
Secure API Management: API keys are stored securely.
Offline Caching: Read articles even without an internet connection.
Responsive UI: Smooth and modern UI built with Jetpack Compose.

---

## Architecture

### Presentation Layer (Module: `app`)

- Built with Jetpack Compose for a reactive UI.
- ViewModels manage UI state.
- Navigation handled by Navigation Compose.

### Domain Layer (Module: `domain`)

- Contains core business logic.
- Defines data models, repository interfaces, and use cases.
- Framework-independent for easy testing.

### Data Layer (Module: `data`)

- Implements repositories defined in the domain layer.
- Uses Retrofit for API calls.
- Uses Room Database for caching and favorites management.
- Handles mapping between API responses and domain models.

---

## Technologies Used

- Kotlin
- Jetpack Compose
- Retrofit
- Room Database
- Dagger Hilt
- Kotlin Coroutines & Flow
- Coil (for image loading)

---

## Screenshots

![Home Screen](assets/images/screenshots\ (1).png) ![Article Detail](assets/images/screenshots\ (2).png) ![Favorites Screen](assets/images/screenshots\ (3).png) ![Search Screen](assets/images/screenshots\ (4).png) ![Error Handling](assets/images/screenshots\ (5).png) ![Offline Caching](assets/images/screenshots\ (6).png) ![Categories](assets/images/screenshots\ (7).png) ![Dark Mode](assets/images/screenshots\ (8).png)

---

## How to Run

1. Clone the repository:

```bash
git clone <your-repo-link>
```

2. Open the project in **Android Studio**.
3. Add your **NewsAPI key** in `local.properties`:

```
NEWS_API_KEY=your_api_key_here
```

---

## Future Improvements

- Add news categories (Technology, Sports, Health, etc.)
- Push notifications for breaking news
- Dark mode support
- Improved offline caching with pagination

---

Created with ❤️ by [M Tayyab & Umar Draz]
