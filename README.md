<div align="center">
  
# Inboxie

**An Action-Intelligent Email Client for Reducing Missed Follow-ups and Deadlines**

[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev/)
[![Firebase](https://img.shields.io/badge/firebase-ffca28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)

*Inboxie surfaces the emails that actually matter based on inferred intent, urgency, and required action—keeping your inbox clean and your mind clear.*

</div>

---

## Abstract & Objectives

Traditional email clients sort by time; Inboxie sorts by **action**. 

Inboxie is a modern, cross-platform email client that augments your inbox with a privacy-aware intelligence layer. Instead of a chronological list of noise, Inboxie instantly identifies emails that require your attention to prevent missed replies, overlooked requests, and dropped deadlines.

- **Action-First Design**: Identify emails that require user action using rule-based and AI-assisted intent detection.
- **Explainable AI**: Understand exactly *why* an email was prioritized with high transparency.
- **Customizable Workflows**: Organize emails by human-readable intents (e.g., Needs Reply, Waiting on Others).
- **Privacy-Aware**: Configurable data storage modes ensure your personal data stays on the device.

---

## Screenshots


<p align="center">
  <img src="https://github.com/neha-n-git/inboxie-portfolio/blob/main/screenshots/splash.png?raw=true" alt="Splash Screen" width="200" />
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://github.com/neha-n-git/inboxie-portfolio/blob/main/screenshots/home.png?raw=true" alt="Main Inbox Screenshot" width="200" />
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://github.com/neha-n-git/inboxie-portfolio/blob/main/screenshots/ai_features.png?raw=true" alt="AI Insights Screenshot" width="200" />
  &nbsp;&nbsp;&nbsp;&nbsp;
  <img src="https://github.com/neha-n-git/inboxie-portfolio/blob/main/screenshots/profile&settings.png?raw=true" alt="Settings Screenshot" width="200" />
</p>

---

## Core Features

### Action-Centric Inbox
A dedicated **"Needs Action"** panel acts as your daily command center. It filters out newsletters and casual chatter, displaying only high-priority emails with smart summary lines. Quickly execute actions: Reply, Snooze, Mark as Done, or Mute Sender.

### Explainable Intelligence
No black boxes. Every flagged email includes a **"Why recommended?"** chip that explains the AI's reasoning. Triggers include:
- Direct questions aimed at you
- Unanswered threads
- Time-sensitive language or hard deadlines

### Intent-Based Buckets
Inboxie auto-sorts your mail into meaningful buckets:
- Needs Reply
- Waiting on Others
- Calendar-worthy
- Bills & Receipts
- Low Value / Newsletters

### Privacy Controls
You control how your data is handled. Choose from:
- **Process-only**: No local storage.
- **Metadata and Summaries**: (Recommended) Fast caching without storing the body.
- **Full Storage**: Complete email text cached for offline use.

---

## System Architecture

Inboxie is built with modern, scalable technologies:

- **Frontend**: Flutter (Material Design 3, Reactive State Management)
- **Backend**: Firebase Authentication (Google Sign-In), Cloud Firestore, Cloud Functions
- **Integrations**: Gmail API (Read-only MVP)
- **Intelligence Layer**: Rule-based intent detection coupled with Groq (LLaMa 3) for ultra-fast summarization and draft assistance.

---

## Getting Started

Want to run Inboxie locally? Follow these steps:

### Prerequisites
- [Flutter SDK](https://docs.flutter.dev/get-started/install) (Stable)
- Android Studio / Xcode
- A [Firebase Project](https://console.firebase.google.com/)
- A [Groq API Key](https://console.groq.com/) for AI features

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/inboxie-portfolio.git
   cd inboxie-portfolio/app
   ```

2. **Install Dependencies**
   ```bash
   flutter pub get
   ```

3. **Configure Environment Variables**
   Currently, AI features require a Groq API key. You can supply this at runtime in the app's Settings page, or configure it via standard Flutter `.env` practices.

4. **Connect Firebase**
   - Register the app in your Firebase project.
   - Download the `google-services.json` (Android) and `GoogleService-Info.plist` (iOS) and place them in their respective native folders.

5. **Run the App**
   ```bash
   flutter run
   ```

---

## Contributing

Contributions, issues, and feature requests are welcome! 
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

