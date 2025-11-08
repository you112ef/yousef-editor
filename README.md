# Yousef Editor

An Android application named "yousef editor" configured to work in mobile screen display mode.

## Features

- Mobile-optimized interface
- Configured for mobile screen display
- Ready to build APK via GitHub Actions

## Building the APK

The project includes a GitHub Actions workflow that automatically builds the APK when code is pushed to the main branch.

### Manual Build

To build the APK locally:

```bash
./gradlew assembleRelease
```

The APK will be generated at:
`app/build/outputs/apk/release/app-release.apk`

## App Configuration

- **App Name**: yousef editor
- **Package Name**: com.yousef.editor
- **Target SDK**: 34 (Android 14)
- **Minimum SDK**: 24 (Android 7.0)

## Project Structure

```
yousef-editor/
├── app/
│   ├── build.gradle
│   ├── proguard-rules.pro
│   └── src/main/
│       ├── java/com/yousef/editor/
│       │   └── MainActivity.kt
│       ├── res/
│       │   ├── layout/
│       │   │   └── activity_main.xml
│       │   ├── values/
│       │   │   ├── colors.xml
│       │   │   ├── strings.xml
│       │   │   └── themes.xml
│       │   ├── xml/
│       │   │   ├── backup_rules.xml
│       │   │   └── data_extraction_rules.xml
│       │   └── mipmap-*/...
│       └── AndroidManifest.xml
├── gradle/wrapper/
├── .github/workflows/
│   └── build.yml
├── build.gradle
├── settings.gradle
├── gradle.properties
└── local.properties
```

## Mobile Display Mode

The app is configured to:
- Work in portrait and landscape orientations
- Adapt to different mobile screen sizes
- Use full screen display mode
- Support both phones and tablets

## License

This project is a modification of the VHEditor-Android project.
