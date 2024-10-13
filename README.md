# Weather App

A simple Weather App built with Flutter that provides real-time weather updates for the current location. The app fetches weather data such as temperature, weather conditions, humidity, and wind speed, using a weather API.

## Features

- **Current Location Weather**: Automatically fetches weather data for the user's current location.
- **Real-Time Weather Updates**: Displays the latest weather information, including temperature, weather condition (sunny, cloudy, rainy, etc.), humidity, and wind speed.
- **User-Friendly Interface**: A clean and simple UI for an intuitive user experience.
- **Location Permission Handling**: Requests location access to provide accurate weather updates.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

- [Flutter SDK](https://flutter.dev/docs/get-started/install) (version 3.0 or above)
- An editor such as [Android Studio](https://developer.android.com/studio) or [VS Code](https://code.visualstudio.com/)
- An API key from a weather data provider like [OpenWeatherMap](https://openweathermap.org/)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/iPriyanshu19/Weather.git
   cd weather-app
   ```

2. **Install dependencies**:
   ```bash
   flutter pub get
   ```

3. **Configure API Key**:
   - Obtain an API key from your chosen weather data provider.
   - Create a `.env` file in the root directory and add the API key:
     ```
     WEATHER_API_KEY=your_api_key_here
     ```
   - Alternatively, you can hardcode the API key in the code, though using environment variables is more secure.

4. **Run the app**:
   ```bash
   flutter run
   ```

## Dependencies

This app uses the following Flutter packages:

- `http`: To make network requests to fetch weather data.
- `geolocator`: To get the current location of the user.
- `flutter_dotenv`: For managing environment variables (API key).
- `provider`: For state management.

Add the following dependencies in your `pubspec.yaml` file:
```yaml
dependencies:
  flutter:
    sdk: flutter
  cupertino_icons: ^1.0.8
  http: ^1.2.2
  geolocator: ^13.0.1
  geocoding: ^3.0.0
  lottie: ^3.1.2
```

## Usage

- **Location Permission**: When the app is launched, it will prompt the user to allow access to the device's location. Grant the permission for the app to function correctly.
- **Weather Information**: The app will then display the current weather details for the detected location.

## Folder Structure

The project follows a simple structure:

```
lib/
│── main.dart           # Entry point of the app
│── models/             # Data models
│── services/           # Services for fetching weather and location data
└── pages/              # Different UI screens
```

## API Integration

- Make sure to sign up for a weather API (like OpenWeatherMap) and get an API key.
- The app makes requests to the weather API to fetch the current weather data for the user's location.


## Contributing

Feel free to submit issues, fork the repository, and send pull requests!