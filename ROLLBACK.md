# Rollback Instructions - TorStream APK

The `main` branch always carries the latest release. Every prior release
is preserved on its own long-lived branch so you can roll back without
losing history.

| Version | Date | Branch | Notes |
|---------|------|--------|-------|
| v2.1 (latest) | 2026-07-12 | `main` | "Play in Player" chooser |
| v2.0 | 2026-06-13 | `backup-stable-v2` | Background download fix |
| v1.0 | 2026-06-10 | `backup-stable-v1` | Initial release |

## If v2.1 Has Issues

### Option 1: Download from Backup Branch (easiest)

1. Visit the GitHub repository: https://github.com/imviren/TorStream-APK
2. Click the branch selector (it currently shows `main`) and pick
   `backup-stable-v2` (or `backup-stable-v1` if you want the very first
   release).
   - Or open the branch directly:
     - https://github.com/imviren/TorStream-APK/tree/backup-stable-v2
     - https://github.com/imviren/TorStream-APK/tree/backup-stable-v1
3. Click on `TorStream.apk`, then "Download".
4. Uninstall the current version from your device and install the
   downloaded APK.
5. Grant the usual permissions.

### Option 2: Use Git Commands (developers)

```bash
# Clone the repository
git clone https://github.com/imviren/TorStream-APK.git
cd TorStream-APK

# Roll back to v2.0 (background download fix)
git checkout backup-stable-v2
# The stable APK is at TorStream.apk

# Or roll back all the way to v1.0 (initial release)
git checkout backup-stable-v1
```

## Comparison Table

| Feature | v2.1 (Latest) | v2.0 (Stable) | v1.0 (Initial) |
|---------|---------------|---------------|----------------|
| "Play in Player" chooser | ✅ Yes | ❌ No | ❌ No |
| Background downloads | ✅ Yes | ✅ Yes | ❌ No |
| Progress notification | ✅ Yes | ✅ Yes | ❌ No |
| Pause/Resume controls | ✅ Yes | ✅ Yes | ❌ No |
| Auto stall recovery | ✅ Yes | ✅ Yes | ❌ No |
| Battery optimization | ✅ Yes | ✅ Yes | ❌ No |
| File size | 64.2 MB | 66.8 MB | 61.2 MB |
| Status | 🟡 Testing | 🟢 Stable | 🟠 Deprecated |

## When to Rollback

Consider rolling back to v2.0 if you experience on v2.1:
- App crashes or freezes
- "Play in Player" chooser doesn't appear
- Downloads not starting
- Battery drain issues
- Notification problems
- Any unexpected behavior

## Reporting Issues

Before rolling back, please report the issue:
1. Go to: https://github.com/imviren/TorStream-APK/issues
2. Click "New Issue"
3. Describe the problem, your Android version, and the version you were on
4. Steps to reproduce

## Re-upgrading to v2.1

Once the issue is fixed:
1. Uninstall the rollback version
2. Switch back to the `main` branch on GitHub
3. Download the new `TorStream.apk`
4. Install and grant permissions
5. Your previous downloads should still be available

## Backup Your Downloads

Before any version change:
1. Note your active download magnet links
2. Completed downloads are stored in:
   - `/Downloads/Antigravity/` folder
3. These files remain safe during version changes

## Support

- Issues: https://github.com/imviren/TorStream-APK/issues
- Branches: https://github.com/imviren/TorStream-APK/branches
