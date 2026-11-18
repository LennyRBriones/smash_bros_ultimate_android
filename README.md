# Smash Characters

An Android guide to the fighters of **Super Smash Bros. Ultimate**: browse the full roster, search by name and open each character's details.

## Stack

- **Kotlin** and **Jetpack Compose**
- **MVVM** with a repository and a single `StateFlow` of UI state
- **Hilt** for dependency injection
- **Retrofit** against the public [Super Smash Bros. Ultimate API](https://super-smash-bros-ultimate-api.onrender.com/)
- **Coil** for images, including SVG
- **Navigation Compose**
- **Firebase** Analytics and Crashlytics

## Structure

```
app/src/main/java/com/lennrbriones/smashcharacters/
├── data/         # Retrofit API
├── repository/   # data access for the view model
├── viewmodels/   # CharactersViewModel
├── state/        # UI state
├── views/        # Home, character detail and search screens
├── components/   # shared Compose components
├── navigation/   # navigation graph
└── di/           # Hilt modules
```

## Building

Open the project in Android Studio and run the `app` configuration. Firebase needs a `google-services.json` in `app/`, which is not committed; download your own from the Firebase console, or remove the Firebase plugins to build without it.
