# KM2

## Project Overview

KM2 is an Android mobile exam practice application developed using web technologies. The project adopts a hybrid development approach (Hybrid App), packaging responsive web pages built with Bootstrap into a native mobile application via Cordova.

Primarily designed for exam preparation scenarios, the application offers features such as simulated exams, timed scoring, categorized project display, and user settings.

## Core Features

- **Simulated Exam System**: Includes a real-time timer, progress bar, score tracking, penalty deduction, and exam completion workflow.
- **Project Card Management**: Displays different categories of exam items in card format (color-coded red/yellow/blue/green), with a clear and intuitive interface.
- **Personal Settings**: Provides basic application configuration options (e.g., toggles for sound and vibration).
- **Interactive Community**: Integrates a contact page featuring QR code display and video popup functionality.
- **UI/UX Design**: Features a modern glassmorphism-styled navigation bar, complemented by the Bootstrap 5 icon library.

## Technology Stack

- **Frontend Technologies**: HTML5, CSS3 (Bootstrap 5 + custom styles), JavaScript
- **UI Framework**: [Bootstrap 5](https://getbootstrap.com/) (CSS & JS)
- **Icon Library**: [Bootstrap Icons](https://icons.getbootstrap.com/)
- **Packaging Framework**: [Apache Cordova](https://cordova.apache.org/)
- **Target Platform**: Android

## Project Structure

```
.
├── config.xml                 # Cordova configuration file
├── my-release-key.keystore    # Android app signing key
├── package.json               # Project dependency configuration
├── static/                    # Static resources directory
│   └── logo/                  # App icons (PWA Icon)
└── www/                       # Frontend source code directory
    ├── assets/
    │   ├── fonts/             # Icon font files
    │   ├── images/            # Image resources (Logo, QR code, etc.)
    │   ├── scripts/           # JavaScript scripts (Bootstrap Bundle)
    │   └── style/             # CSS style files
    ├── index.html             # Homepage / exam entry point
    ├── km3.html               # Exam module page
    ├── contact.html           # Contact page
    └── profile.html           # Profile page
```

## Quick Start

1. **Environment Setup**:
   - Install [Node.js](https://nodejs.org/)
   - Install [Android SDK](https://developer.android.com/studio#command-line-tools)
   - Globally install Cordova: `npm install -g cordova`

2. **Build Android APK**:
   ```bash
   # Install dependencies
   npm install
   
   # Add Android platform
   cordova platform add android
   
   # Build Release package (requires signing configuration)
   cordova build android --release
   ```

## License

This project is licensed under the applicable open-source or commercial license (see the LICENSE file in the root directory).