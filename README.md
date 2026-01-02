 * ======================================================================================
 * PROJECT: ESP32 8-Channel Smart Switch with Timer & Schedule
 * ======================================================================================
 * 
 * DESCRIPTION:
 * This program turns an ESP32 into a web-controlled smart switch for 8 distinct devices.
 * It features a responsive web interface, physical button controls, countdown timers, 
 * and a daily schedule. It uses Non-Volatile Storage (Preferences) to remember settings,
 * Wi-Fi credentials, and relay states even after a power failure.
 * 
 * KEY FEATURES:
 * 1. Web Interface: Control 8 relays, set timers, and configure schedules via browser.
 * 2. Physical Controls: Support for 8 physical push buttons with software debouncing.
 * 3. Persistence: Remembers Relay State, WiFi Creds, and Schedules after reboot.
 * 4. Smart Timer: Resumes countdown after power loss (if time sync is successful).
 * 5. Timekeeping: NTP (Network Time Protocol) to get accurate time from the internet.
 * 6. Optimization: Disables Access Point (AP) mode once connected to WiFi to save CPU/Power.
 * 
 * HARDWARE PINS:
 * - Relays: GPIO 23, 22, 21, 19, 18, 5, 17, 16
 * - Buttons: GPIO 32, 33, 25, 26, 27, 14, 13, 4
 * 
 * LIBRARIES REQUIRED:
 * - WiFi.h, WebServer.h (Standard ESP32 libs)
 * - Preferences.h (Standard ESP32 lib for storage)
 * - ESPmDNS.h (For resolving .local names)
 * ======================================================================================
