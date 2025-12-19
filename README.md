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

![Screenshot](https://paksource.info/wp-content/uploads/2025/12/screenshots-1.png)

---

## Future Improvements

- Add news categories (Technology, Sports, Health, etc.)
- Push notifications for breaking news
- Dark mode support
- Improved offline caching with pagination

---

Created with ❤️ by [M Tayyab & Umar Draz]
