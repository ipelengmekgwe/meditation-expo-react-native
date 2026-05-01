# Meditation App

A guided meditation timer for iOS and Android, built with Expo and React Native.

## Stack

- **Framework:** Expo SDK 51, React Native, TypeScript
- **Navigation:** Expo Router (file-based)
- **Styling:** NativeWind (Tailwind for React Native)
- **Audio:** expo-av for ambient sound playback
- **State:** React context + AsyncStorage for session history
- **Tooling:** EAS Build for native binaries

## What it does

A small, deliberate app for short meditation sessions:

- Pick a duration (1, 3, 5, 10, 15 minutes) and an ambient sound (rain, forest, white noise, silence).
- A timer with smooth circular progress runs the session; gentle haptics signal start, mid-point, and end.
- Sessions are stored locally so the home screen can show a streak and a "minutes this week" stat.
- Light & dark themes follow the device.

The point isn't to be a full meditation platform — it's to be one nice screen that does one thing well, and to learn Expo Router + NativeWind in the process.

## Running locally

```bash
npm install
npx expo start
# Press `i` for iOS sim, `a` for Android emulator, or scan the QR with Expo Go
```

To produce installable binaries:

```bash
npx eas build --profile preview --platform ios
npx eas build --profile preview --platform android
```

## Status

In active development — core timer + sound flow works. Streak / history tracking and onboarding are next.

---

Part of [Ipeleng's portfolio](https://github.com/ipelengmekgwe/portfolio).
