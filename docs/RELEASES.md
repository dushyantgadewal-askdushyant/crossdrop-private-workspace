# Public Release Notes

## 1.0.41 — 2026-10-11

Brand consistency patch: Android legacy and adaptive launcher icons now use the
approved CrossDrop infinity-transfer mark rather than the Flutter/Dart icon.
The Android launcher artwork uses the same master mark as Windows, on a light
brand surface for reliable contrast.

This package is prepared for device-launcher verification before public
distribution. The earlier file labelled 1.0.40+42 is withdrawn because it
contained stale 1.0.39+41 Android metadata and must not be distributed.

The verified replacement asset is `CrossDrop-Android-1.0.41+43.apk` with
SHA-256:

`683D9495460548D71873E0BC9A01A603B42F838859865A958DA97CDC7C3A7903`

## 1.0.39 — 2026-10-11

Early-access validation release for Windows and Android.

### Highlights

- Encrypted local pairing, direct files/batches, and messages between supported
  devices.
- QR and code pairing alongside local-network discovery.
- Trusted-device management and conservative automatic-file controls.
- Android request notifications for pairing, messages, and file approval while
  CrossDrop is minimized or locked, when keep-ready is enabled.
- Android foreground transfer progress and cancellation for active file
  transfers.
- Windows tray presence, installer updates, and internal signing.

### Download assets for the first public release

| Platform | Asset | SHA-256 | Distribution note |
| --- | --- | --- | --- |
| Android | `CrossDrop-Android-1.0.39+41.apk` | `8670BC8C1D04FE248BC87BA9B36B903FA95DB8F6A8E7E7C132377DE7C7CE6810` | Direct APK; Android may require permission to install from this source. |
| Windows | `CrossDrop-Setup-1.0.39-internal.exe` | `7EAEEFB671CA9BED80126AAE4CE91F535179A2A5F9FA1B393AFFD5ABD5801F86` | Internally self-signed; Windows can show a trust warning until a publicly trusted signing certificate is used. |

### Known limitations

- CrossDrop currently supports Windows and Android distribution only.
- Devices must be able to reach one another on a private local network; normal
  internet access alone is not sufficient.
- Interrupted transfers safely stop and can be sent again, but do not yet resume
  from the exact byte at which they stopped.
- Android keep-ready requires a visible quiet system notification. Force-stopping
  CrossDrop ends its local listener.

### Before publishing this release

- Upload only the files listed above to an official GitHub Release.
- Recalculate checksums after any rebuild.
- Confirm the version, package name, screenshots, and changelog match.
- Do not label the Windows installer as publicly trusted while it uses the
  internal certificate.
