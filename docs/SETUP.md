# Dev Environment Setup

A step-by-step guide to getting GravelMapper running on your machine.

---

## 1. Install Node.js

Download and install Node.js v18+ from https://nodejs.org/
Verify it works:
```bash
node --version
```

## 2. Install Expo CLI

```bash
npm install -g expo-cli
```

## 3. Install the Expo Go app on your phone

- iPhone: search "Expo Go" in the App Store
- Android: search "Expo Go" in the Play Store

## 4. Get a Mapbox token

1. Create a free account at https://mapbox.com
2. Go to your Account page
3. Copy your **Default public token**

## 5. Set up Supabase

1. Create a free account at https://supabase.com
2. Create a new project
3. Go to Settings → API
4. Copy your **Project URL** and **anon public key**

## 6. Configure your environment

```bash
cp .env.example .env
```

Open `.env` and paste in your tokens.

## 7. Install dependencies and run

```bash
npm install
npx expo start
```

Scan the QR code in your terminal with the Expo Go app.

---

## Helpful VS Code Extensions

- **React Native Tools** — debugging support
- **Prettier** — code formatting
- **ESLint** — catch errors early
- **GitLens** — better GitHub integration
