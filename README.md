# Android App: NetScope X

This project is a ready-to-open Android WebView app that hosts the NetScope X network diagnostics interface and adds a bulk scan engine for many IPs and DNS names.

## Features
- Browser-like diagnostics UI
- Batch target scanning with unlimited manual entries
- Default large IP/DNS sample lists
- Support for IP range expansion like `192.168.1.20-192.168.1.60`
- Optional delay between requests for sequential scan
- DOH-style DNS resolution and HTTP checks
- Prepared for arm64 APK generation

## Build
1. Open with Android Studio.
2. Let Gradle sync.
3. Build -> Build Bundle(s) / APK(s) -> Build APK(s).
4. The APK will be generated under `app/build/outputs/apk/debug/` or `release/`.

## Notes
- This app is a WebView wrapper. Real network access depends on device permissions and remote endpoint availability.
- For production-like security, different checks should be moved to native Android code or a trusted backend.
