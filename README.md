# Geofence Tracker App

A Flutter application for tracking geofences with background location updates and notifications using SharedPreferences.

## Setup Instructions

1. Clone the repository
2. Run `flutter pub get` to install dependencies
3. For Android:
    - Ensure you have Google Maps API key and add it to `android/app/src/main/AndroidManifest.xml`
    - Build APK: `flutter build apk`
4. For iOS:
    - Ensure you have a Mac with Xcode
    - Update `ios/Runner/Info.plist` with your Google Maps API key
    - Open `ios/Runner.xcworkspace` in Xcode
    - Build and run on simulator or device

## Example

| HomeScreen                                                                                             | Add Geofence Screen                                                                                    | Geofence History                                                                                      |
|--------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------|
| <img src="https://ik.imagekit.io/6ilngyaqa/1747481518559-Screenshot_2025_0517_165548_FzUuXtMXxI.jpg"/> | <img src="https://ik.imagekit.io/6ilngyaqa/1747481595940-Screenshot_2025_0517_165558_x1Jm4Ub7pM.jpg"/> | <img src="https://ik.imagekit.io/6ilngyaqa/1747481636052-Screenshot_2025_0517_165607_Dm5va3QC5.jpg"/> |



## Required Dependencies

- flutter
  - cupertino_icons: ^1.0.8
  - get: ^4.7.2
  - logger: ^2.5.0
  - fluttertoast: ^8.2.12
  - location: ^8.0.0
  - flutter_local_notifications: ^19.2.0
  - flutter_background_service: ^5.1.0
  - google_maps_flutter: ^2.12.1
  - geolocator: ^9.0.2
  - permission_handler: ^12.0.0+1
  - shared_preferences: ^2.5.3
  - rxdart: ^0.28.0
  - intl: ^0.19.0
  - flutter_polyline_points: ^2.1.0

## Testing Guidelines

1. Launch the app and grant location permissions
2. Add a geofence using the "+" button
3. Move to trigger enter/exit events
4. Check history screen for movement logs
5. Verify notifications are received
6. Test edit/delete functionality

## Notes

- Google Maps API key is required
- Ensure proper permissions are granted
- Background location tracking may impact battery life
- SharedPreferences is used for local storage
```