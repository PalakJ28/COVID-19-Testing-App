# COVID-19 Testing App

A comprehensive Android application designed to help users during the COVID-19 pandemic by providing testing capabilities, symptom tracking, and quarantine support.

## 📱 Project Overview

The COVID-19 Testing App is an Android-based application that helps users navigate the challenges of the COVID-19 pandemic. It provides essential tools for symptom assessment, safety information, and quarantine activities to support users during lockdown periods.

##  Key Features

### 🔍 COVID-19 Testing & Detection
- **Symptom Assessment**: Interactive questionnaire-based testing to identify potential COVID-19 symptoms
- **Risk Analysis**: AI-powered analysis to predict infection likelihood
- **Multi-language Support**: Test available in English, Hindi, and Gujarati

### Real-time Information
- **Live Patient Counter**: Real-time COVID-19 patient statistics
- **Help Centers**: Locate nearby COVID-19 testing and treatment centers
- **Notifications**: 2-hour interval sanitization reminders

### Safety & Prevention
- **Symptom Information**: Comprehensive guide to COVID-19 symptoms
- **Prevention Measures**: Detailed safety protocols and precautions
- **Health Guidelines**: Best practices for staying safe during the pandemic

### 🏠 Quarantine Support
- **Quarantine Activities**: Curated list of activities to make quarantine time productive
- **Mental Health Support**: Activities designed to maintain mental well-being during isolation

## Technical Stack

### Frontend
- **Language**: Java (Android)
- **UI Framework**: Android XML Layouts
- **Design Components**: Material Design Components
- **Animations**: Lottie animations for enhanced UX

### Backend & Dependencies
- **HTTP Client**: Volley for network requests
- **UI Components**: RecyclerView, CardView, ConstraintLayout
- **Text Processing**: JustifyText library for better text formatting
- **Testing**: JUnit and Espresso for unit and UI testing

### Build System
- **Build Tool**: Gradle 4.0.1
- **Minimum SDK**: API 23 (Android 6.0)
- **Target SDK**: API 29 (Android 10)
- **Compile SDK**: API 29

##  Prerequisites

Before running this project, ensure you have:

- **Android Studio** (latest version recommended)
- **Java Development Kit (JDK)** 8 or higher
- **Android SDK** with API level 23 or higher
- **Gradle** (included with Android Studio)

## Installation & Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd COVID-19-Testing-App
   ```

2. **Open in Android Studio**
   - Launch Android Studio
   - Select "Open an existing Android Studio project"
   - Navigate to the project directory and select it

3. **Sync Gradle**
   - Android Studio will automatically sync the project
   - If not, click "Sync Now" in the notification bar

4. **Build and Run**
   - Connect an Android device or start an emulator
   - Click the "Run" button (green play icon) or press `Shift + F10`

## App Structure

```
COVID-19-Testing-App/
├── app/
│   ├── src/main/
│   │   ├── java/           # Java source code
│   │   ├── res/            # Resources (layouts, strings, drawables)
│   │   ├── assets/         # Static assets
│   │   └── AndroidManifest.xml
│   ├── build.gradle        # App-level build configuration
│   └── proguard-rules.pro  # Code obfuscation rules
├── gradle/                 # Gradle wrapper files
├── build.gradle           # Project-level build configuration
├── settings.gradle        # Project settings
└── README.md              # This file
```

## Configuration

### API Configuration
The app uses Volley for network requests. Ensure you have proper internet permissions in your `AndroidManifest.xml`:

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```

### Language Support
The app supports three languages:
- English (default)
- Hindi
- Gujarati

Language resources are stored in the `res/values-*` directories.

## Testing

The project includes comprehensive testing:

- **Unit Tests**: Located in `app/src/test/`
- **Instrumented Tests**: Located in `app/src/androidTest/`
- **UI Tests**: Using Espresso framework

To run tests:
```bash
# Unit tests
./gradlew test

# Instrumented tests
./gradlew connectedAndroidTest
```

## Building for Release

1. **Generate signed APK**
   - Go to `Build` → `Generate Signed Bundle / APK`
   - Choose `APK`
   - Create or select a keystore
   - Choose `release` build variant

2. **Build using command line**
   ```bash
   ./gradlew assembleRelease
   ```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request




