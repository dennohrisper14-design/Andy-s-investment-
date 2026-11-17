# RentMaster Android starter

This is an Android Studio project for the first RentMaster phone-app prototype.

## What works in this prototype
- Dashboard with rent, occupancy and maintenance summaries
- Add and save buildings, tenants, rent payments and maintenance requests
- Kenyan shilling (KSh) display
- Data is saved locally on this phone using browser storage inside the app

## Important limitations
This is the first working prototype, not the finished live rental platform.
- Data is only stored on the device; it does not sync between phones or users.
- There is no real login, cloud database, tenant invitation or M-Pesa payment processing yet.
- Do not use it as the official record for real tenant payments until cloud sync, authentication, backups and security checks are added.

## Build the APK
### Option 1: Android Studio
1. Install Android Studio on a computer.
2. Open this folder as an existing project.
3. Allow Gradle sync to finish.
4. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. Android Studio will show the location of the debug APK.

### Option 2: GitHub Actions
The project includes `.github/workflows/build-apk.yml`.
1. Create a GitHub repository and upload all files in this folder.
2. Open the repository's **Actions** tab.
3. Run **Build RentMaster Android APK** (or push to the `main` branch).
4. Open the completed workflow run and download the `RentMaster-debug-apk` artifact.
5. Extract the APK and install it on your Android phone. Android may ask you to allow installation from that source.

The APK produced by this workflow is a debug/testing build, not a Play Store release.
