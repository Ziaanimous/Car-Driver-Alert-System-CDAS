CAR DRIVER ALERT SYSTEM (CDAS)
==============================

Description:
------------
A Flutter app that monitors driver drowsiness using face detection and provides real-time alerts to prevent accidents. The app uses the device's front camera to continuously monitor the driver's face for signs of drowsiness such as closed eyes or yawning. When drowsiness is detected, the app triggers visual, audio, and haptic alerts to wake the driver up.

Features:
---------
1. Real-time Face Detection:
   - Uses Google ML Kit Face Mesh Detection to monitor driver's face
   - Detects drowsiness through eye closure detection
   - Detects yawning through mouth opening detection

2. Multi-modal Alerts:
   - Visual alerts on screen
   - Audio alerts with customizable sounds
   - Haptic feedback (vibration)
   - Bluetooth-connected external alert device support
   - Picture-in-Picture (PIP) overlay alerts

3. Driving Analytics:
   - Tracks total alerts and high alarms
   - Calculates safe driving score
   - Provides driving statistics and recommendations
   - Usage percentage tracking

4. User Authentication:
   - Login/Registration functionality
   - User profile management

5. Bluetooth Integration:
   - Connect to external alert devices
   - Bluetooth settings and tutorial screens

6. Customizable Settings:
   - Alert preferences (sound, vibration, notifications)
   - Sensitivity levels
   - Auto-start scan option

7. Data Visualization:
   - Charts for driving statistics
   - Detailed analytics dashboard

How It Works:
-------------
1. The app uses your device's front camera to monitor your face.
2. Advanced algorithms detect signs of drowsiness like closed eyes or yawning.
3. When drowsiness is detected, the app triggers visual and audio alerts.
4. Statistics are collected to help you understand your driving patterns.

Key Screens:
------------
1. Launch Screen - Initial app screen with loading indicators
2. Login/Signup Screen - User authentication
3. Welcome Screen - Post-authentication welcome message
4. Home Screen - Main monitoring interface with camera preview
5. Data Screen - Driving statistics and analytics
6. Settings Screen - App configuration and user profile
7. Bluetooth Settings - Device connection management
8. Tutorial Screens - Usage guides and instructions

Technical Implementation:
-------------------------
- Face Detection: Google ML Kit Face Mesh Detection
- Camera: flutter camera package
- Audio: audioplayers package
- Bluetooth: flutter_blue_plus package
- Charts: syncfusion_flutter_charts package
- State Management: Provider package
- Persistent Data: Shared preferences
- PIP Overlay: system_alert_window package

Note: The app requires camera permissions to function properly. For Bluetooth alerts, an external device must be paired and connected.