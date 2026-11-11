# 8Ball Assist (Android)

A small Android overlay prototype for 8 Ball Pool. It draws a user-controlled aiming ray and an optional simple bank-shot guide over other apps.

## Important limitation
This first version is a **manual overlay**, not an automatic Aiming Master clone. It does not inspect the game screen, detect balls, calculate collision paths, or guarantee pocket predictions. The guide is a movable reference line that you rotate in 5-degree steps.

## Build the APK
1. Install Android Studio (current stable) and Android SDK Platform 35.
2. Open this `8BallAssist` folder in Android Studio and let Gradle sync.
3. Choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. Android Studio will show the generated APK location (normally `app/build/outputs/apk/debug/app-debug.apk`).

## Install and use
1. Install the APK on Android.
2. Open **8Ball Assist** and tap **Grant overlay permission**. Enable “Display over other apps”.
3. Return to the app and tap **Start aiming overlay**.
4. Open 8 Ball Pool. Drag the overlay header to move its control panel.
5. Use −5° / +5° to rotate the guide, **Bank** to show a basic reflected guide, **Hide lines** to toggle the drawing, and **Close** to stop it.

The app requests overlay permission explicitly and runs a foreground service while active. Android may show a persistent notification.
