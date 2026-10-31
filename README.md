# EduScore Android Test

This is a small, safe packaging test. It is NOT your full school management system.

## What it tests
- Packaging a web app into an Android APK using Capacitor.
- Opening the app without Google AI Studio.
- Saving a small test note locally on the device.
- Showing whether the device is online or offline.

## Build the APK without installing Android Studio on your laptop

1. Create or sign in to a GitHub account.
2. Create a new repository, for example `eduscore-android-test`.
3. Extract this ZIP file on your computer.
4. Upload all extracted files and folders to the repository (the `.github` folder must also be uploaded).
5. Open the repository's **Actions** tab.
6. Select **Build EduScore Test APK**.
7. Press **Run workflow** (or push to the `main` branch).
8. Wait for the workflow to finish successfully.
9. Open the completed workflow run and download the `EduScore-Test-APK` artifact.
10. Extract the downloaded artifact ZIP. It contains `app-debug.apk`.
11. Transfer `app-debug.apk` to your Android phone and install it. Android may ask you to allow installation from that source.

## Test it
- Open EduScore Test.
- Type a note and press **Save on this device**.
- Close the app fully and reopen it. The note should still be there.
- Turn on airplane mode and reopen it. The test screen should still load.

## Important limitations
- This is only a demonstration wrapper, not the real EduScore system.
- It does not connect to Firebase or Gemini.
- It does not include student, teacher, attendance or result records.
- It is an unsigned debug APK for testing, not a Play Store release.
- Do not use real student information in this test.

## Next step
Once this test APK installs and opens successfully on your phone, the same packaging process can be applied to the real EduScore project after reviewing its security, backend requirements, and offline synchronization.
