# Privacy Policy for HatSwap

**Last Updated:** March 24, 2026

At **HatSwap**, we believe that your digital habits and the apps you use are your business. Our "Privacy First" philosophy means the app is designed to function entirely on your device without a central server or routine data collection.

## 1. Data Collection and Usage
- **Local-only data:** HatSwap stores all user-created content (Hats, schedules, app associations, and preferences) locally on your device using Room and Jetpack DataStore. The app does not send this data to any server by default.
- **No accounts or tracking:** You are not required to create an account or provide an email address. HatSwap does not include analytics, tracking pixels, or third‑party marketing SDKs.

Note: The app currently does not use a separate on‑device encryption library (e.g., SQLCipher or AndroidX Security) for the Room database. If encryption-at-rest is added in a future release, we will update this policy to describe the implementation.

## 2. Permissions and Device Features
HatSwap requests a small set of system permissions or settings access to enable its core features. All requests are for on‑device use only.

- **Installed apps / package visibility:** HatSwap enumerates launcher apps using the system PackageManager (e.g., `queryIntentActivities(...)`) so you can pick apps for your Hats. The app does not currently declare the broad `QUERY_ALL_PACKAGES` permission in the manifest. The list of apps is used only locally to populate the App Picker and is never uploaded or shared. If we later add `QUERY_ALL_PACKAGES`, we will document that change and provide the required Play Console justification.

- **Usage Access (`PACKAGE_USAGE_STATS`):** HatSwap may ask you to grant Usage Access in system settings to support schedule detection or to determine the currently active/foreground app in certain flows. This access must be enabled manually by the user in Settings and the related data is processed on‑device only.

- **Overlay / Draw over apps (`SYSTEM_ALERT_WINDOW`):** If you enable features that require on‑screen overlays, HatSwap may request the Draw‑over‑apps permission. This is an optional user setting that must be enabled in system Settings and is used only for the described UX; overlay content and related events are not transmitted off‑device.

## 3. Backups and Export/Restore
- **Device backups:** HatSwap sets `android:allowBackup="false"` to avoid automatic cloud backups to the device account. This prevents routine device cloud backup from including your HatSwap data.
- **Local export/import:** We provide an explicit local backup and restore flow (export/import JSON) you can use to move or preserve your data. Exports are written to locations you choose and are not sent to our servers.

## 4. Third‑Party Services and Feedback
- **No analytics or crash-reporting SDKs:** HatSwap does not include analytics, advertising, or crash‑reporting SDKs (for example: Firebase Analytics/Crashlytics, Sentry, Bugsnag). If we add any third‑party telemetry in the future, we will update this policy and list the services and the exact data they collect.

- **Feedback via GitHub:** When you use the in‑app feedback action, HatSwap opens a GitHub Issue URL and may prefill non‑identifying technical metadata (Device model, Android OS version, App version). You can review and edit this information before submitting; nothing is posted until you complete the GitHub submission.

## 5. Data Deletion and Control
- **Delete / clear data:** All HatSwap data is stored in your app sandbox. Uninstalling the app or using the system "Clear data" control removes local HatSwap data from your device. You can also delete or export data from within the app if that feature is provided.
- **Assistance:** If you need help deleting or exporting data, contact us via the GitHub feedback link in the app and we will assist.

## 6. Children’s Privacy
HatSwap does not knowingly collect personal information from children. Because the app does not collect or transmit personal user data by default, it is compliant with the Children’s Online Privacy Protection Act (COPPA).

## 7. Changes to This Policy
We may update our Privacy Policy from time to time. We will notify users of changes by posting the updated Privacy Policy on this page and updating the "Last Updated" date.

## 8. Contact Us
If you have any questions or suggestions about our Privacy Policy, please contact us via the GitHub feedback link within the app.