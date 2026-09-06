# Kalladai Borewell – Flutter Android App

This project converts the supplied **Borewell at Kalladai.xlsx** workbook into a Flutter Android app.

## Included
- Dashboard
- Detailed Estimate
- EB Materials
- PVC & GI Materials
- Sub Estimate
- Reports / totals
- Search
- Add, edit and delete estimate/material items
- Automatic amount calculation (quantity × rate)
- Local persistence on Android
- Reset to the original Excel-imported dataset
- GitHub Actions workflow that builds a release APK automatically

## Cloud build
Upload the **contents** of this ZIP to a GitHub repository. Then open **Actions → Build Android APK → Run workflow**.

The workflow automatically creates the missing Android/Gradle wrapper files, runs `flutter pub get`, builds the release APK, and uploads the APK as an Actions artifact named `kalladai-borewell-apk`.

## Local build
If using a 64-bit development computer:
```bash
flutter pub get
flutter run
flutter build apk --release
```
