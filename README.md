# Movie Finder App (Flutter)

## Overview

Movie Finder is a Flutter application that allows users to explore popular, new, and searched movies using The Movie Database (TMDb) API. Users can view movie details and receive random movie suggestions. This project serves as a portfolio piece to showcase Flutter development skills.

## Features

* Browse lists of popular movies.
* Discover movies currently playing in theaters.
* Search for specific movies by title.
* View detailed information for each movie (description, poster, rating, release date).
* Get a random movie suggestion.
* Seamlessly navigate between different sections.

## Screenshots

*Add screenshots of your app here!*

* [Home Screen Screenshot]
* [Detail Screen Screenshot]
* [Search Results Screenshot]
* [Random Movie Suggestion Screenshot]

## Tech Stack & Dependencies

* **Framework:** Flutter
* **Programming Language:** Dart
* **State Management:** flutter_riverpod
* **HTTP Client:** http
* **API:** The Movie Database (TMDb) API
* **JSON Handling:** dart:convert / (optional: json_serializable)

## Installation & Usage

### Prerequisites

* Flutter SDK: [Installation Guide](https://docs.flutter.dev/get-started/install)
* A TMDb API Key: Obtain one for free at [TMDb Website](https://www.themoviedb.org/signup)

### Steps

1. **Clone the repository:**
    ```bash
    git clone [Your GitHub Repository Link Here]
    cd movie_finder_app
    ```

2. **Configure the API Key:**
    * Create a file named `constants.dart` in the `lib` directory.
    * Add the following content, replacing `'YOUR_API_KEY_HERE'` with your actual TMDb API key:
        ```dart
        // lib/constants.dart
        const String tmdbApiKey = 'YOUR_API_KEY_HERE';
        ```
    * **IMPORTANT:** Add `lib/constants.dart` to your `.gitignore` file to prevent exposing your API key on GitHub. Add the following line to `.gitignore`:
        ```
        /lib/constants.dart
        ```

3. **Install dependencies:**
    ```bash
    flutter pub get
    ```

4. **Run the app:**
    ```bash
    flutter run
    ```

## Project Structure (Example)

```
lib/
├── main.dart           # App entry point
├── constants.dart      # API key (IMPORTANT: add to .gitignore!)
├── models/             # Data models (e.g., movie.dart)
│   └── movie.dart
├── providers/          # Riverpod providers
│   └── movie_providers.dart
├── screens/            # UI screens
│   ├── home_screen.dart
│   ├── detail_screen.dart
│   └── search_screen.dart
├── services/           # API interaction logic
│   └── tmdb_api_service.dart
└── widgets/            # Reusable UI components
    └── movie_list_item.dart
```

---

*Created by Nikolaos Sporidis*