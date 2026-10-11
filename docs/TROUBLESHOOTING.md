# Troubleshooting

## Devices cannot see each other

1. Ensure both devices are on the same private local network.
2. Open CrossDrop on both devices; on Android, enable **Keep CrossDrop ready
   while minimized** when testing while locked or away from the app.
3. Refresh the Devices page.
4. Avoid guest Wi-Fi and networks with client/AP isolation enabled.
5. Use **Show my QR** / **Scan QR** or **Join with code** if discovery does not
   find the other device.

Internet access alone does not prove that devices can contact one another.
Routers, extenders, guest networks, and network isolation can keep devices on
different local segments.

## A trusted device is shown offline

- Confirm CrossDrop is running on the other device, or that Android keep-ready
  is enabled.
- Refresh the Devices list.
- Check both devices use the same local Wi-Fi/LAN and are not connected through
  a guest network.
- Review the trusted-device details for last-seen and endpoint information.
- If the device identity changed unexpectedly, do not continue until you have
  confirmed the change with the owner of the other device.

## Android notifications do not arrive

1. In Android Settings inside CrossDrop, enable **Keep CrossDrop ready while
   minimized**.
2. Allow CrossDrop's Android notification permission.
3. Confirm the quiet ongoing “CrossDrop is ready” notification remains visible.
4. Do not force-stop the app or swipe it away if you expect it to listen.
5. Review Android battery restrictions if your device manufacturer aggressively
   stops background apps.

## A transfer stops

The sender and receiver remain safe if Wi-Fi is interrupted, either app exits,
or the receiver rejects the request. Reconnect the devices and send a new
offer. Keep the original source file until you confirm the received copy opens
correctly.

## Before asking for help

Share the app version, platform, a short sequence of steps, and the visible
error text. Remove file names, file contents, QR codes, pairing codes, device
IDs, local IP addresses, and other personal information from public reports.
