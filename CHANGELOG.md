## 1.1.0
- Added Swift Package Manager support on iOS (CocoaPods still supported for projects that have not migrated).
- Converted the iOS plugin to pure Swift, removing the Objective-C shim.
- Fixed web plugin registration pointing at a non-existent `flutter_sms_web.dart` file.
- Fixed iOS crash when `sendSMS` is invoked with malformed method-channel arguments (replaced force cast with a guarded cast returning a `bad_arguments` error).
- Phone numbers are now URI-encoded when building `sms:` launch URLs, preventing recipient strings from injecting extra query parameters.
- Renamed the Android package from the `com.example.send_message` placeholder to `com.ioagra.send_message`.

## 1.0.2
- Added iOS platform support.

## 1.0.1

* SMS and MMS for Android and iOS
