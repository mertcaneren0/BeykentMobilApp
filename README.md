# BeykentMobilApp

The first UI skeleton of an Android campus app prototype for Beykent University.

## Overview

A small Java Android app with a role picker (Student, Academic, Staff). Each role opens a login screen, and the login button goes straight to that role's home screen. There is no authentication or data yet; this version sets up the navigation, layouts, colors and custom font. The UI is in Turkish.

It is the starting point of the same project:

1. **BeykentMobilApp** (this repo): first UI skeleton
2. [BeykentMobileApp2](https://github.com/mertcaneren0/BeykentMobileApp2): full screen set with static content and demo logins
3. [BeykentUniversitesiMobil](https://github.com/mertcaneren0/BeykentUniversitesiMobil): final version, wired to Firebase Auth and Realtime Database, with an admin panel

## Screens

- Role picker (`MainActivity`)
- Student, academic and staff login screens
- Student, academic and staff home screens

## Tech

- Java, Android SDK (compileSdk / targetSdk 29, minSdk 21, build tools 29.0.2)
- Android Gradle Plugin 3.5.3
- AndroidX AppCompat 1.1.0, ConstraintLayout 1.1.3

## Project structure

```
app/
  build.gradle
  src/main/java/com/mertcaneren/beykentmobilapp/
    MainActivity.java       role picker
    *GirisLogin.java        login screens
    *AnaSayfa.java          home screens
  src/main/res/             layouts, drawables, custom font
```

## Build and run

1. Clone the repo and open the root folder in Android Studio.
2. Let Gradle sync. The project uses an old Gradle/AGP setup (AGP 3.5.x), so a recent Android Studio may ask you to upgrade the Gradle wrapper or plugin.
3. Run on an emulator or device with Android 5.0 (API 21) or newer.

## Notes

This is a student/learning project and not an official Beykent University app.

---

Built by [Mertcan Eren](https://github.com/mertcaneren0)
