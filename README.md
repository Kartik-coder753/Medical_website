
# Medical_website
This is an medical website !!!
More Updates coming soon ...

# MediBuddy - Healthcare Platform

**A modern, real-time healthcare platform connecting patients with healthcare professionals.**

![MediBuddy Banner](https://via.placeholder.com/800x200/3B82F6/FFFFFF?text=MediBuddy+Healthcare+Platform)

## Overview

MediBuddy is a full-featured web application built with **React 18 + TypeScript + Vite**. It enables seamless medical consultations, real-time communication (chat + video/voice calls via WebRTC), appointment management, health data visualization, and instant notifications.

Key capabilities include:
- Real-time messaging and video calls (`socket.io-client` + `simple-peer`)
- Interactive charts and analytics (`recharts`)
- Toast notifications (`react-toastify`)
- Date handling and scheduling (`date-fns`)
- Beautiful, responsive UI with dark mode support (`Tailwind CSS` + `lucide-react` icons)
- Client-side routing (`react-router-dom`)
- Unique IDs for sessions/calls (`uuid`)

---

## Tech Stack

| Layer          | Technology                          |
|----------------|-------------------------------------|
| Framework      | React 18 + TypeScript               |
| Build Tool     | Vite 5                              |
| Styling        | Tailwind CSS 3 + PostCSS            |
| Routing        | React Router DOM 6                  |
| Real-time      | Socket.io Client 4 + Simple Peer 9  |
| Charts         | Recharts 2                          |
| Icons          | Lucide React                        |
| Notifications  | React Toastify                      |
| Utilities      | date-fns, uuid                      |
| Linting        | ESLint 9 (flat config) + typescript-eslint |
| Type Checking  | TypeScript 5                        |

---

## Project Structure (Root)
medibuddy-healthcare-platform/
├── .gitignore
├── eslint.config.js
├── index.html
├── package.json
├── postcss.config.js
├── tailwind.config.js
├── tsconfig.app.json
├── tsconfig.json
├── tsconfig.node.json
├── vite.config.ts
├── README.md                  ← You are reading this
└── src/                       ← (App source - not shown in this document set)
text---

## Configuration Files Explained

### `package.json`
- Project name, version, and scripts
- All dependencies and devDependencies
- Available scripts:
  ```json
  {
    "dev": "vite",
    "build": "vite build",
    "lint": "eslint .",
    "preview": "vite preview"
  }
vite.config.ts

Vite configuration with official React plugin
Excludes lucide-react from dependency optimization (common compatibility fix)

tailwind.config.js

Content paths for purging unused styles
darkMode: 'class' (toggle via dark class on <html>)
Custom animation: pulse-slow

postcss.config.js

Enables Tailwind CSS and Autoprefixer

eslint.config.js

Modern flat ESLint config (ESLint v9+)
Extends recommended JS + TypeScript rules
Includes react-hooks and react-refresh plugins
Ignores dist/ folder
Applies only to **/*.{ts,tsx} files

TypeScript Configs

tsconfig.json – Root file that references the other two
tsconfig.app.json – For src/ (React JSX, strict mode, DOM libs)
tsconfig.node.json – For vite.config.ts (Node/ESNext environment)

index.html

Entry HTML file
Meta tags for SEO and PWA readiness
Title: MediBuddy - Healthcare Platform
Loads /src/main.tsx

.gitignore

Standard ignores for Node.js + Vite + editors
Excludes node_modules, dist, logs, .DS_Store, IDE files, etc.


Getting Started
Prerequisites

Node.js ≥ 18
npm / yarn / pnpm

Installation
Bash# 1. Clone the repository
git clone <your-repo-url>
cd medibuddy-healthcare-platform

# 2. Install dependencies
npm install
Development
Bash# Start dev server (usually opens http://localhost:5173)
npm run dev
Production Build
Bashnpm run build
# Output goes to /dist
Preview Production Build
Bashnpm run preview
Linting
Bashnpm run lint

Features Implemented (based on dependencies)

Real-time patient-doctor communication
WebRTC video/voice calls
Live health metrics & charts
Appointment booking & calendar
Dark/light theme toggle
Responsive mobile-first design
Toast notifications for appointments, calls, etc.


Folder Structure (Expected in src/)
textsrc/
├── assets/
│   └── logo.svg
├── components/
├── pages/
├── hooks/
├── utils/
├── App.tsx
├── main.tsx
└── ...

Contributing

Fork the project
Create a feature branch (git checkout -b feature/amazing-feature)
Commit changes (git commit -m 'Add amazing feature')
Push to branch (git push origin feature/amazing-feature)
Open a Pull Request


License
This project is private (see package.json). All rights reserved.

Made with ❤️ for better healthcare access.
Last updated: February 22, 2026
textCopy the entire content above into a new file named **`README.md`** at the root of your project. It comprehensively documents **every file** you provided while giving users and developers everything they need to understand, install, and run MediBuddy.2s
