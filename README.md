# Wifi-Smart_Switch_Control

   ===========================================
 * PROJECT: ESP32 4-Channel Smart Switch with Timer & Schedule
 * ===========================================
 * 
 * DESCRIPTION:
 * This program turns an ESP32 into a web-controlled smart switch for 4 distinct devices.
 * It features a responsive web interface, physical button controls, countdown timers, 
 * and a daily schedule. It uses Non-Volatile Storage (Preferences) to remember settings,
 * Wi-Fi credentials, and relay states even after a power failure.
 * 
 * KEY FEATURES:
 * 1. Web Interface: Control 4 relays, set timers, and configure schedules via browser.
 * 2. Physical Controls: Support for 4 physical push buttons with software debouncing.
 * 3. Persistence: Remembers Relay State, WiFi Creds, and Schedules after reboot.
 * 4. Smart Timer: Resumes countdown after power loss (if time sync is successful).
 * 5. Timekeeping: NTP (Network Time Protocol) to get accurate time from the internet.
 * 6. Optimization: Disables Access Point (AP) mode once connected to WiFi to save CPU/Power.
 * 
 * HARDWARE PINS:
 * - Relays: GPIO 26, 27, 14, 12
 * - Buttons: GPIO 16, 17, 18, 19
 * 
 * LIBRARIES REQUIRED:
 * - WiFi.h, WebServer.h (Standard ESP32 libs)
 * - Preferences.h (Standard ESP32 lib for storage)
 * - ESPmDNS.h (For resolving .local names)
 * ===========================================


🔥 New Project Release: 4-Channel ESP32 Web Controller

Hi everyone! I’ve developed a robust firmware for the ESP32 to control 4 relays with full scheduling and timer capabilities. It features a responsive Web UI and a dedicated Web Installer for easy flashing.

⚙️ Specs & Features:
Channels: 4x Relays (Active LOW) + 4x Manual Buttons.
Zero-Coding Setup: Flash directly from the browser using Web Serial.
mDNS Support: Access via 
http://smart-switch-control.local
 (no IP hunting!).
On-Board Scheduling: Saves schedules to flash memory (works even after reboot).
Time Sync: Automatic NTP time synchronization.

🛠️ How to get started:
Connect your ESP32 Dev Module via USB.
Go to the Web Installer: [LINK TO YOUR GITHUB PAGE]
Click "CONNECT & INSTALL".
Connect to WiFi 
ESP32-Relay-Config
 to setup your network.

🔌 Pinout:
Relays: GPIO 26, 27, 14, 12
Buttons: GPIO 16, 17, 18, 19
