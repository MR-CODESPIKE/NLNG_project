# NLNG Project

NLNG Project is an Android application prototype built with Gradle and Kotlin/Java Android tooling. The project uses a conventional `app/` module and includes the Android build wrapper, resources, and application configuration needed for Android Studio development.

## Build and run

```bash
./gradlew assembleDebug
```

Open the repository root in Android Studio, allow Gradle to sync, and run the debug variant on an emulator or connected device. The supported SDK and language levels are defined in `app/build.gradle`; keep the local JDK aligned with that configuration.

## Layout

| Path | Purpose |
|---|---|
| `app/` | Android application module. |
| `app/src/main/` | Kotlin/Java sources, manifest, and resources. |
| `build.gradle` | Root build configuration. |
| `settings.gradle` | Project and module inclusion. |
| `gradlew` | Reproducible Gradle wrapper entry point. |

## Status

This is an early project repository. The source tree should be treated as the authority for implemented features; this README intentionally avoids promising functionality that is not represented in the current module. Before distributing an APK, document the application ID, permissions, backend configuration, supported devices, test coverage, and release-signing process.

Do not commit secrets, local SDK paths, generated APKs, or user data. Use build variants or an untracked local configuration file for environment-specific endpoints.
