# TorStream-APK
Public download host for the TorStream Android APK

## 📱 Latest Version

### v2.1 - Web Stream Media Player Chooser (Latest)
- **File**: `TorStream.apk` (also archived as `TorStream-v2.1-webstream-chooser.apk`)
- **Size**: 64.2 MB
- **Build Date**: July 12, 2026
- **Features**:
  - ✅ "Play in Player" button on every torrent details screen — opens Android's system media-player chooser (VLC, MX Player, system player, Kodi, …) and hands the Webtor stream URL to the picked player
  - ✅ Webtor "Web Stream" button still available (in-app WebView player)
  - ✅ Background downloads with persistent progress notification (carried over from v2.0)
  - ✅ Pause / Resume / Stop controls from the notification
  - ✅ Automatic stall detection and recovery
  - ✅ Battery optimization exemption support

### v2.0 - Background Download Fix
- **File**: `TorStream-v2-background-fix.apk`
- **Backup Branch**: `backup-stable-v2`
- **Features**:
  - ✅ Background downloads now work when app is minimized
  - ✅ Persistent notification with download progress
  - ✅ Pause/Resume/Stop controls from notification
  - ✅ Automatic stall detection and recovery
  - ✅ Battery optimization exemption support

### v1.0 - Stable Release (Archived)
- **File**: `TorStream.apk` (on `backup-stable-v1` branch)
- **Backup Branch**: `backup-stable-v1`
- **Status**: ⚠️ Known issue: Downloads stop when app is backgrounded

## 🔽 Download Instructions

1. **For New Users**: Download `TorStream.apk` from the `main` branch (always the latest)
2. **Existing Users**: Update to v2.1 for the new "Play in Player" feature
3. **Need to Rollback**: See `ROLLBACK.md` or download from one of the backup branches below

## 🔄 Installation

1. Download the APK file
2. Enable "Install from Unknown Sources" in Android settings
3. Open the downloaded APK file
4. Grant necessary permissions when prompted
5. Start downloading torrents!

## 📋 Permissions Required

- **Storage**: Save downloaded files
- **Network**: Download torrents
- **Notifications**: Show download progress
- **Background Service**: Continue downloads when app is minimized

## 🐛 Known Issues

### v2.1
- None reported yet — testing in progress

### v2.0
- No known issues

### v1.0
- ❌ Downloads stop when switching apps
- ❌ No background download support
- ❌ No notification controls

## 📦 Version History

| Version | Date | Size | Status | Notes |
|---------|------|------|--------|-------|
| v2.1 | 2026-07-12 | 64.2 MB | 🟡 Testing | "Play in Player" chooser |
| v2.0 | 2026-06-13 | 66.8 MB | 🟢 Stable  | Background download fix |
| v1.0 | 2026-06-10 | 61.2 MB | 🟠 Deprecated | Initial release |

## 🔧 Rollback Instructions

If v2.1 has issues, you can rollback to v2.0 (or v1.0):

1. Go to GitHub repository
2. Switch to the relevant branch:
   - `backup-stable-v2` for the v2.0 background-fix release
   - `backup-stable-v1` for the v1.0 initial release
3. Download `TorStream.apk` from that branch
4. Uninstall the current version and install the older one

For full rollback instructions see `ROLLBACK.md`.

## 📝 Build Information

- **Min SDK**: Android 7.0 (API 24)
- **Target SDK**: Android 15 (API 35)
- **Architecture**: Universal (ARM + x86)
- **Signing**: Release keystore (`torstream-release.jks`)

## 📞 Support

Report issues at: https://github.com/imviren/TorStream-APK/issues
