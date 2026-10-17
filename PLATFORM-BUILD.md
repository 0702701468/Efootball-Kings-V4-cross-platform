# eFootball Kings Online v4 — Platform Build

This package is the real v4 cross-platform source base derived from the v3 application.

## Web
- Vite builds the existing eFootball Kings browser app into `dist/`.
- `vercel.json` is included for static Vercel hosting.
- Run `npm install`, then `npm run build`.
- Deploy the repository/project root to Vercel.

## Supabase
The app still uses the existing Supabase schema and browser-safe anon key. Do not place a service-role key in frontend code.

For the current static implementation, set the values in `public/config.js` before deployment, or adapt the config to your deployment environment.

## Android
After Node/npm and Android Studio are installed:
1. `npm install`
2. `npm run cap:add:android`
3. `npm run cap:sync`
4. `npx cap open android`
5. Build an APK for testing or an AAB for Google Play.

The Android project is intentionally generated locally because the Android SDK/Gradle environment is machine-specific.

## Windows / macOS / Linux
Tauri configuration is included under `src-tauri/`.

After Rust and the platform prerequisites are installed:
- `npm install`
- `npm run desktop:build`

Windows produces an installer/bundle from the Tauri build; macOS/Linux can be built on their respective supported environments.

## Existing functionality preserved
The v4 package keeps the v3 Supabase-powered workflow: authentication, players, competitions, seasons, fixtures, result submission, screenshot evidence, admin approval, standings, player management, and PWA assets.
