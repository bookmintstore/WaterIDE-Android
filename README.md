# WaterIDE Android APK build

This project packages the supplied WaterIDE HTML prototype into a fullscreen Android WebView app. It does not require Android Studio on your computer; GitHub Actions builds the APK in the cloud.

## Build
1. Create a GitHub repository named `WaterIDE-Android`.
2. Upload all files and folders from this project to the repository root (including the hidden `.github` folder).
3. Open the repository's **Actions** tab and enable Actions if prompted.
4. Select **Build WaterIDE APK** and click **Run workflow**. A push to `main` also triggers a build.
5. Open the completed workflow run. Under **Artifacts**, download `WaterIDE-debug-APK` and unzip it to get `app-debug.apk`.
6. Transfer `app-debug.apk` to your Android phone and install it. You may need to allow installation from your browser or file manager.

## Important
- This is a demo wrapper. Motor controls and water readings remain simulated until the real ESP32/backend is integrated.
- This is a debug APK for testing, not a Play Store release. Keep the repository private if you do not want to publish your prototype source code.
