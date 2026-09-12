# Privacy Policy for HatSwap

**Last Updated:** September 12, 2026

At **HatSwap**, we believe that your digital habits and the apps you use are your business. Our "Privacy First" philosophy means the app is designed to function entirely on your device without a central server or routine data collection.

## 1. Data Collection and Usage
- **Local-only data:** HatSwap stores all user-created content (Hats, schedules, app associations, and preferences) locally on your device using Room and Jetpack DataStore. The app does not send this data to any server by default.
- **No accounts or tracking:** You are not required to create an account or provide an email address. HatSwap does not include analytics, tracking pixels, or third‑party marketing SDKs.

Note: The app currently does not use a separate on‑device encryption library (e.g., SQLCipher or AndroidX Security) for the Room database. If encryption-at-rest is added in a future release, we will update this policy to describe the implementation.

## 2. Permissions and Device Features
HatSwap requests a minimal set of system permissions to enable its core scheduling and widget features. All permissions are used strictly on-device:

- **Installed apps / package visibility:** HatSwap enumerates launcher apps using Android's standard `<queries>` declaration and `PackageManager` so you can choose apps for your Hats. The app does not request broad package visibility (`QUERY_ALL_PACKAGES`) or Usage Access (`PACKAGE_USAGE_STATS`). The list of installed apps is queried and displayed entirely on your device and is never transmitted off-device or shared.

- **Exact Alarms (`SCHEDULE_EXACT_ALARM` / `USE_EXACT_ALARM`):** HatSwap uses exact alarm permissions exclusively to trigger your scheduled hat switches at the precise times you configure. HatSwap does not collect or transmit any data through the alarm system.

- **Battery Optimization Exclusion (`REQUEST_IGNORE_BATTERY_OPTIMIZATIONS`):** To prevent Android's battery saver (Doze mode) from delaying or suppressing scheduled hat switches, HatSwap may request to be excluded from battery optimizations. This is handled via standard Android system dialogs and processes no user data.

- **Device Boot (`RECEIVE_BOOT_COMPLETED`):** Required to automatically restore your active hat state and reschedule your user-defined alarms whenever your device reboots.

## 3. Backups and Export/Restore
- **Device backups:** HatSwap sets `android:allowBackup="false"` to avoid automatic cloud backups to the device account. This prevents routine device cloud backup from including your HatSwap data.
- **Local export/import:** We provide an explicit local backup and restore flow (export/import JSON) you can use to move or preserve your data. Exports are written to locations you choose and are not sent to our servers.

## 4. Third‑Party Services and Feedback
- **No analytics or crash-reporting SDKs:** HatSwap does not include analytics, advertising, or crash‑reporting SDKs (for example: Firebase Analytics/Crashlytics, Sentry, Bugsnag). If we add any third‑party telemetry in the future, we will update this policy and list the services and the exact data they collect.

- **Feedback via Email:** When you use the in‑app feedback action, HatSwap opens your device's email application with a pre-filled draft addressed to `support@sosiacollective.com`. The draft includes non-sensitive diagnostic details (Device model, Android OS version, and HatSwap version) to help troubleshoot issues. You have complete control to review, edit, or delete any of this information before sending; nothing is transmitted until you choose to send the email.

## 5. Data Deletion and Control
- **Delete / clear data:** All HatSwap data is stored in your app sandbox. Uninstalling the app or using the system "Clear data" control removes local HatSwap data from your device. You can also delete or export data from within the app if that feature is provided.
- **Assistance:** If you need help deleting or exporting data, contact us via email at `support@sosiacollective.com` and we will assist.

## 6. Children’s Privacy
HatSwap does not knowingly collect personal information from children. Because the app does not collect or transmit personal user data by default, it is compliant with the Children’s Online Privacy Protection Act (COPPA).

## 7. Changes to This Policy
We may update our Privacy Policy from time to time. We will notify users of changes by posting the updated Privacy Policy on this page and updating the "Last Updated" date.

## 8. Contact Us
If you have any questions or suggestions about our Privacy Policy, please contact us via email at `support@sosiacollective.com`.