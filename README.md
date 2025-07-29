# Dynamic Battery Notifier for Android

A Tasker-based utility to provide advanced, customizable, and beautifully animated battery notifications for Android devices.

<p align="center">
  <video width="432" autoplay loop muted playsinline>
    <source src="demo.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</p>

## The Problem
Standard Android battery notifications are often generic and lack context. They typically provide a single, simple alert for low battery and full charge, without distinguishing between different levels of urgency or providing a rich user experience.

## The Solution
This project replaces the native system with a fully custom-tailored notification engine built within Tasker. It provides distinct visual and auditory feedback for multiple battery states, both when discharging and charging, enhancing user awareness and improving battery health management.

## Core Features
*   **Multi-Level Alerts:** Triggers unique notifications for 6 different battery states (5%, 15%, 25% discharging & 85%, 90%, 100% charging).
*   **Context-Aware Logic:** Utilizes distinct logic for charging vs. discharging states, ensuring the correct alert is always shown.
*   **Custom Animated UI:** A sleek, "Dynamic Island" style popup built with HTML, CSS, and SVG provides a modern and visually appealing alert. The UI is populated with live data from Tasker.
*   **Intelligent Screen Wake:** For charging notifications when the screen is likely off, the system uses a high-priority notification to wake the screen smoothly to the lock screen without glitches.
*   **Varied User Feedback:**
    *   **Discharging Alerts (Screen On):** Plays a notification sound and provides haptic feedback (vibration) without a persistent notification in the status bar.
    *   **Charging Alerts (Screen Off):** Creates a high-priority notification in the status bar to wake the device.
*   **Battery Health Logging:** Includes a secondary feature to log charging start/stop times and key battery milestones for user review.

## Technology Stack
*   **Automation Engine:** [Tasker](https://tasker.joaoapps.com/)
*   **User Interface:** HTML5, CSS3 (Flexbox, Keyframes, CSS Variables), SVG
*   **Logic:** Tasker's built-in logic gates, variable management, and system state detection.

## How to Use
1.  Ensure you have the Tasker app installed on your Android device.
2.  Download the `Dynamic_Battery_Notifier.prj.xml` file from this repository.
3.  In Tasker, long-press on the "Home" icon (or any project tab) and select "Import Project".
4.  Navigate to and select the downloaded `.xml` file.
5.  Tasker will import all required Profiles, Tasks, and Scenes. Enable the profiles to begin using the system.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
