# eFootball Kings Online v4

Cross-platform eFootball competition platform for the web, Android and desktop.

## Included
- Existing Supabase-powered player/competition workflow from v3
- Vite production web build
- Vercel deployment configuration
- Capacitor Android configuration
- Tauri desktop configuration for Windows/macOS/Linux
- PWA manifest and service worker
- Supabase schema and setup SQL

## Quick start
```bash
npm install
npm run dev
```

Production build:
```bash
npm run build
npm run preview
```

## Supabase
Configure `public/config.js` with the Supabase project URL and **anon/public key only**. Never expose a service-role key.

## Platform builds
See `docs/PLATFORM-BUILD.md` for Android and desktop packaging.

## Deployment
Deploy the project root to Vercel after configuring Supabase.
