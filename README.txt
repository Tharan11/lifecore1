LIFECORE V4 — COMPLETE OFFLINE-FIRST WELLNESS PWA
================================================

WHAT THIS BUILD INCLUDES
- Responsive V3-derived dashboard and existing wellness journals
- V3 localStorage migration: reads lifecore_v3 and creates lifecore_v4
- Running/walking/workout logs, meal journal, hydration, sleep and habits
- Foreground GPS session tracker with route preview (HTTPS + location permission required)
- Mood and energy journal
- Wellness calendar and daily summaries
- Offline LIFECORE Intelligence summaries (no external AI calls)
- Achievements and CSV/JSON exports
- Backup restore and privacy controls
- English, Tamil and Hindi base interface from V3
- Dark/light theme, PWA installation and offline service worker cache

IMPORTANT PLATFORM SCOPE
This is a cross-platform Progressive Web App (PWA), not a native Expo/React Native app.
It can be used in modern browsers and installed on compatible Android/iOS devices.
It does NOT include native Health Connect / Apple HealthKit integrations, reliable background
GPS, native background notifications, cloud accounts or cross-device sync. Those require
separate native/platform integrations and real-device configuration/testing.
The GPS feature is foreground-only and requires HTTPS or localhost. Do not rely on it as a
medical or emergency tracking device.
The AI Coach is deterministic and local; it does not call a remote AI model.
Data is stored in this browser profile. Other people with access to the profile may access it.
Export backups and keep them private. No app can guarantee data recovery after browser data
is cleared unless the user has an external backup.

V3 DATA MIGRATION
On first launch, V4 reads existing lifecore_v3 localStorage data if no V4 data exists,
normalises the known V3 collections, then saves a copy as lifecore_v4. The V3 key is not
deleted. This migrates browser-local records only; it cannot access records from another
device or a different browser origin.

RUN LOCALLY
1. Extract this ZIP.
2. Open a terminal in the extracted folder.
3. Run: python -m http.server 8000
4. Visit http://localhost:8000
For GPS, test on localhost or a deployed HTTPS address.

FREE WEB DEPLOYMENT
1. Create a GitHub repository.
2. Upload the contents of this folder to its root.
3. Open Settings > Pages.
4. Choose Deploy from a branch, branch main, folder /(root), then Save.
5. Open the HTTPS Pages URL and install from the browser menu.

ANDROID / IOS
Install as a PWA from Chrome (Android) or Safari (iOS) where supported.
This package is not an APK, IPA, or app-store submission.
Native app-store releases require a separate native build, signing, permissions,
store review and real-device testing. iOS App Store distribution may require paid Apple
developer membership. Do not assume all capabilities are available through a PWA.

SAFETY
LIFECORE is a general wellness journal, not a medical device or medical service.
It does not diagnose, prescribe, set restrictive calorie goals, or recommend extreme exercise.
Stop activity if you feel unwell and seek help from a trusted adult/qualified professional
for personal health concerns.
