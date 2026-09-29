# GymTrack

GymTrack is a mobile-first fitness tracker for building workout plans, logging exercise details, tracking daily hydration, and reviewing progress. The interface supports English and Arabic, including a right-to-left Arabic layout.

## Live site

[Open GymTrack](https://leyn767.github.io/gymtrack/) (published with GitHub Pages).

## Features

- Account creation, login, logout, and profile onboarding
- Daily workouts with editable exercises, sets, reps, weight, notes, reordering, and completion tracking
- Searchable exercise library with categories and difficulty levels
- Eight ready-made workout plans
- Rest timer for training sessions
- Daily water tracking with a configurable goal and quick-add controls
- Workout history, streaks, activity charts, hydration consistency, and weight tracking
- English and Arabic language selector, remembered in the browser
- Responsive desktop navigation and mobile bottom navigation

## Tech stack

GymTrack is a static single-page application built with HTML, CSS, and vanilla JavaScript. It has no build step or third-party JavaScript dependencies. Arabic and English copy live in separate locale bundles under `outputs/locales/`.

## Run locally

Open `outputs/index.html` in a modern browser, keeping the `outputs/locales/` directory beside it. Or serve the project locally with Python:

```sh
python3 -m http.server 8000
```

Then open [http://localhost:8000/outputs/](http://localhost:8000/outputs/).

## Data and authentication

The current prototype stores account records and app data in browser `localStorage`. This keeps a session and personal workout data available after refresh in the same browser profile. It is not server-backed authentication, and data does not sync between devices. Do not use a real or reused password. A production multi-user deployment should use a trusted authentication provider and server-side database with per-user access controls.

## Screenshots

Add screenshots here after capturing the application. Suggested views:

- Home dashboard
- Workout planner and exercise library
- Water tracker
- Progress page
- Arabic right-to-left layout
