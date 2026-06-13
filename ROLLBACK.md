# Rollback Instructions - TorStream APK

## If v2.0 Has Issues

If you experience problems with the new v2.0 APK with background download support, you can easily rollback to the stable v1.0 version.

## Quick Rollback Guide

### Option 1: Download from Backup Branch

1. **Go to GitHub Repository**
   - Visit: https://github.com/imviren/TorStream-APK

2. **Switch to Backup Branch**
   - Click on the branch selector (usually shows "main")
   - Select `backup-stable-v1` branch
   - Or go directly to: https://github.com/imviren/TorStream-APK/tree/backup-stable-v1

3. **Download Stable APK**
   - Click on `TorStream.apk`
   - Click "Download" button
   - File size: 61.2 MB

4. **Install v1.0**
   - Uninstall v2.0 from your device
   - Install the downloaded v1.0 APK
   - Grant necessary permissions

### Option 2: Use Git Commands (Developers)

```bash
# Clone the repository
git clone https://github.com/imviren/TorStream-APK.git
cd TorStream-APK

# Checkout backup branch
git checkout backup-stable-v1

# The stable APK is available as TorStream.apk
```

## Comparison Table

| Feature | v2.0 (New) | v1.0 (Stable) |
|---------|-----------|---------------|
| Background Downloads | ✅ Yes | ❌ No |
| Progress Notification | ✅ Yes | ❌ No |
| Pause/Resume Controls | ✅ Yes | ❌ No |
| Auto Stall Recovery | ✅ Yes | ❌ No |
| Battery Optimization | ✅ Requests Exemption | ❌ None |
| File Size | 66.8 MB | 61.2 MB |
| Status | 🟡 Testing | 🟢 Stable |

## When to Rollback

Consider rolling back to v1.0 if you experience:
- App crashes or freezes
- Downloads not starting
- Battery drain issues
- Notification problems
- Any unexpected behavior

## Reporting Issues

Before rolling back, consider reporting the issue:
1. Go to: https://github.com/imviren/TorStream-APK/issues
2. Click "New Issue"
3. Describe the problem
4. Include your Android version
5. Steps to reproduce

## Re-upgrading to v2.0

Once issues are fixed in v2.0:
1. Uninstall v1.0
2. Download v2.0 from main branch
3. Install and grant permissions
4. Your previous downloads should still be available

## Backup Your Downloads

Before any version change:
1. Note your active download magnet links
2. Completed downloads are stored in:
   - `/Downloads/Antigravity/` folder
3. These files remain safe during version changes

## Support

- Issues: https://github.com/imviren/TorStream-APK/issues
- Branch: https://github.com/imviren/TorStream-APK/tree/backup-stable-v1