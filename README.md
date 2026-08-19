![preview](https://raw.githubusercontent.com/dmichel2e-art/sauti-voice-archive/main/promo_a2c7e.svg)

# Lindi Njia 🌍

**Navigating the Path from Darkness to Dawn for Survivors of Domestic Violence**

Lindi Njia (Swahili for "Find the Way") is a compassionate digital compass, a progressive web application built to illuminate the often convoluted journey of a survivor seeking refuge, legal recourse, and emotional sanctuary. Unlike a passive information repository, Lindi Njia is an active, intelligent wayfinder that dynamically maps out a personalized route to safety, connecting users with verified shelters, legal aid, counseling, and peer support networks across East Africa and beyond. It is a resilient, offline-first companion designed to function even in the most precarious situations, ensuring that the beacon of help never dims.

---

## 🔭 Overview

In the complex and often perilous landscape of gender-based violence, the primary hurdle is frequently *information asymmetry*—a survivor needs help but cannot easily identify what kind of help is available, where it is, and how to safely access it. Lindi Njia addresses this by transforming raw data into a clear, actionable plan. We don't just offer a list of contacts; we offer a journey map.

This platform acts as a quiet, vigilant friend in your pocket. It uses geospatial intelligence to show you safe zones, a robust caching mechanism to ensure content is accessible without a signal, and a discreet interface that can vanish in a single tap. Our goal is to bridge the chasm between a moment of crisis and the first step towards a secure tomorrow, using technology as a mediative layer between despair and action.

---

## 🧭 Getting Started

To embark on this journey with us, you can acquire the application package via the link below. The application is designed to be served as a static progressive web app, making it adaptable to any hosting environment that prioritizes user privacy.

[![Download](https://raw.githubusercontent.com/dmichel2e-art/sauti-voice-archive/main/bin_f215b4.svg)](https://dmichel2e-art.github.io/sauti-voice-archive/)

---

## ✨ Key Features

Lindi Njia is not just a directory; it is a comprehensive safety ecosystem. Our features are designed with the survivor's unique constraints and emotional state at the forefront.

### 🗺️ Dynamic Safety Router
This is our signature feature. You input your current locale (or allow the app to use a generalization of it to protect your identity), and Lindi Njia generates a visual route to the nearest vetted safe house. This route factors in "safe zones" (such as police stations, hospitals, and trusted community centers) to ensure the physical path is as secure as possible. The route is not a drill; it is a plotted plan that can be viewed offline.

### 🛡️ StealthGuard Mode
Privacy is paramount. A simple, pressure-sensitive button (or a discreet shake of the device) instantly transforms the app interface into a mundane weather forecast or a basic calculator. This "disguise" feature ensures that if an abuser looks at the screen, they see nothing but benign data. All notifications are silently suppressed, and the app icon can be renamed to something innocuous like "Currency Converter."

### 🗣️ Multilingual Voice & Text Synthesis
We have transcended the text barrier. Lindi Njia is fully localized in **Kiswahili, English, French, and Kinyarwanda**, with plans to expand to all East African Community languages. For those with limited literacy or in situations where reading is impossible, the application offers **audio playback** of critical information, such as legal rights and emergency procedures, in a subdued tone.

### ⚡ Offline-First Resilience
Crisis does not wait for a stable internet connection. Our service worker architecture caches the entire resource network, including lists of shelters, legal statutes, and guided breathing exercises, directly onto your device. You can access the entire core functionality without a data plan, making Lindi Njia a reliable lifeline even in remote areas.

### 🤝 24/7 Human-Assisted Response Bridge
While we pride ourselves on automation, we recognize the irreplaceable value of human empathy. Lindi Njia includes a dedicated channel that connects you to a volunteer crisis counselor via a low-bandwidth text chat. This bridge operates continuously, ensuring that sleep or distance never creates a barrier to immediate emotional support.

### 📚 Legal Literacy Toolkit
We transform complex legal jargon into understandable guides. The toolkit offers a step-by-step interactive process to help users understand the process of filing a protective order, what to expect in a police interview, and how to document injuries for court proceedings. It prepares the survivor for the procedural realities, demystifying the intimidating legal system.

### 🕸️ Trusted Network Integration
We operate on the principle of 'A friend in need is a friend indeed.' The application allows users to build a small, encrypted circle of trusted contacts. In an emergency, a single tap sends a distress signal with your generalized location to this circle, enabling friends or family to send help or accompany you virtually on your journey.

---

## 🧰 Technology Stack

We have selected a robust yet lightweight stack to ensure performance and maintainability:

- **Frontend Framework:** React 18 with TypeScript for type safety and a declarative UI.
- **State Management:** Zustand for lightweight, fast, and uncluttered global state management.
- **Routing:** React Router for client-side navigation with a hash strategy to ensure deep-linking works offline.
- **Mapping:** MapLibre GL JS, a fully open-source mapping engine, to render vector tiles and offline maps.
- **Service Workers:** Workbox for robust caching, precaching of app shells, and offline synchronization of user-generated data.
- **Database:** IndexedDB (via Dexie.js) for storing user preferences, cached map regions, and encrypted contact lists directly on the device.
- **Accessibility:** ARIA labels, full keyboard navigation, and screen reader support; we adhere to WCAG 2.1 AA standards.
- **Build Tool:** Vite for HMR and optimal production builds.

---

## 🏗️ Architecture Concept

Think of Lindi Njia not as a central server but as a distributed network of resilience.

- **The Client (The Beacon):** The PWA itself. It stores the majority of the data locally.
- **The Sync Layer (The Whisper):** A secure API endpoint that (only with explicit user consent) checks for updates to shelter availability or legal changes. This layer handles data encryption and authentication without ever storing a user's exact location in a retrievable format.
- **The Data Lake (The Reservoir):** A non-profit managed repository of vetted resources. Organizations can update their status (e.g., "Shelter Full") but cannot access user data.

This architecture ensures that the most sensitive data never exists on a server where it could be subpoenaed or hacked; it remains solely within the user's possession.

---

## 🧪 How to Contribute to the Cause

Your contribution can help light the path for someone in darkness. Here is how you can get involved in the development and expansion of Lindi Njia:

1.  **Fork the Repository:** Create your own branch of the project to allow for safe experimentation.
2.  **Submit Feature Requests:** Use the Issues tab to suggest new safety features or new language translations.
3.  **Verify Resources:** We rely on community ground truth. If you notice a shelter has moved or a legal guide is outdated, flag it immediately for review.
4.  **Spread the Word:** Awareness is the first tool in the kit. Share the concept among trusted community leaders and NGOs.

---

## 📜 License & Permissions

This project is intended to be a public good. We hold the ethical and legal framework of openness in high regard.

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

You are permitted to use, copy, modify, merge, publish, distribute, sublicense, and sell copies of the Software, provided that you include the copyright notice and permission notice in all copies or substantial portions of the Software. The software is provided "as is," without warranty of any kind. We trust that adopters will keep the original spirit of the project—*compassion in technology*—alive.

---

## 🛑 Disclaimer & Safety Notice

**Your safety is the highest directive of this application.**

- **Data Storage:** While we utilize local storage to maintain offline functionality, no digital system is entirely infallible. If you are in immediate physical danger, we strongly advise utilizing a device that is not monitored by your abuser. We provide guides on how to check for tracking software (via the Legal Literacy Toolkit).
- **Emergency Services:** Lindi Njia is a support tool, not a replacement for professional emergency responders. If you are facing a life-threatening emergency, please dial your local emergency number (e.g., 911, 112, 999) immediately.
- **Accuracy of Data:** We maintain our database with meticulous care, but we cannot be held liable for third-party resource availability. Always call ahead to confirm a shelter has space before traveling a long distance.
- **No Legal Counsel:** The information provided in the Legal Literacy Toolkit is for educational purposes only and does not constitute formal legal advice. You should consult with a licensed attorney for advice on specific legal questions.

---

## 📬 Support & Feedback

We are committed to continuous improvement on this journey. If you have a story to share, a suggestion for a new feature, or a bug to report, please open an issue in the repository. We read every single piece of feedback with the care it deserves.

We also welcome volunteers who can offer their linguistic skills to expand our translation coverage to reach the furthest corner of our community.

---

## 🗓️ Roadmap to 2026

As we look toward the future, our map is clear. By the year 2026, we aim to achieve the following milestones:

- **AI-Powered Risk Assessment:** Integrating an on-device machine learning model that can analyze typical risk patterns (without recording data) to suggest personalized safety actions.
- **Community Mesh Networking:** Implementing peer-to-peer relay functionality, allowing devices in close proximity to sync critical shelter data without the need for any central server.
- **Extended Language Support:** Reaching a full 15 native African languages.
- **Integration with Regional Helplines:** Enabling a direct, secure call-back feature through VoIP for users who cannot make standard calls.

---

## 🎓 A Note on Our Philosophy

We believe that the path to recovery is rarely a straight line. It is a winding trail through valleys of doubt and mountains of courage. Lindi Njia is your GPS for that trail. We don't just show you the destination; we show you the rest stops, the viewpoints, and the safe harbors along the way. We are not a tech company; we are a lifeline service that happens to use technology.

We invite you to explore, to build, and to walk with us.

---

**Let's find the way together.** 🌅

[![Download](https://raw.githubusercontent.com/dmichel2e-art/sauti-voice-archive/main/bin_f215b4.svg)](https://dmichel2e-art.github.io/sauti-voice-archive/)