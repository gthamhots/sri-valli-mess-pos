SRI VALLI MESS POS — ANDROID APK PROJECT

This is an Android Studio project wrapping the existing Sri Valli Mess billing app in a native Android WebView. It bundles the app locally so billing can open without internet after installation. Bills/menu are saved in the app's WebView local storage on this device.

FEATURES
- Tamil + English menu and billing
- Offline local app assets
- Device-local bill storage and daily reports
- JSON backup and CSV report export to Android Downloads
- Android print dialog for receipts (printer support depends on Android print service / printer)

BUILD IN ANDROID STUDIO
1. On a computer, install Android Studio (stable) and Android SDK Platform 35.
2. Extract this ZIP.
3. Android Studio > Open > choose the extracted Sri_Valli_Mess_Android folder.
4. Wait for Gradle sync and SDK downloads.
5. Build > Build Bundle(s) / APK(s) > Build APK(s).
6. Find APK at app/build/outputs/apk/debug/app-debug.apk. Transfer it to your Android phone, open it, and allow installation from that source if Android asks.

BUILD APK ONLINE (NO LOCAL ANDROID SDK)
1. Create a private or public GitHub repository and upload all files/folders from this project.
2. Open the repository's Actions tab.
3. Run the workflow named “Build Sri Valli Mess APK” (or push a commit).
4. Open the completed workflow run and download the artifact named Sri-Valli-Mess-POS-debug-apk. Extract it to get app-debug.apk.

IMPORTANT
- This ZIP contains source code and an automated build workflow, NOT a precompiled APK. It needs Android Studio or GitHub Actions to compile the APK.
- This is a debug APK for direct installation/testing, not a Play Store release. A Play Store release needs a signed release build.
- Bills stay on this device. Export JSON backups regularly; uninstalling the app or clearing its data can erase bills.
- Test printing, backup export/import, and a sample bill before using for real sales.
