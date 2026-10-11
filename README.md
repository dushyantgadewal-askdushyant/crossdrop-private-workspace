# CrossDrop

**Private files and messages, shared directly between your devices.**

CrossDrop is a local-workspace application for sending files, links, and short
messages between nearby Windows and Android devices. It is designed for people
who want a direct, private transfer experience without an account, cloud drive,
or central relay service.

> This public repository is CrossDrop's product home. It intentionally contains
> documentation, release information, and approved distribution material only;
> it does not contain CrossDrop source code.

## Why CrossDrop exists

CrossDrop began while **Dushyant Gadewal — #AskDushyant** was building
[BlackDemon.IN CreativeAI Universe](https://blackdemon.in). Moving creative
files, reference material, links, and short notes between devices was a
repeated interruption: many familiar sharing and messaging workflows send
content through an internet service before it reaches the intended device.

That can be convenient, but it is not always the right trade-off for founders,
entrepreneurs, creators, and small teams who want clearer control of their
work. In an AI-driven world, privacy is not an afterthought. Data should not
leave a private network without a deliberate choice, clear guardrails, and the
right approval.

CrossDrop is built around that principle:

- keep transfers direct between the devices involved;
- use encrypted sessions for data in transit;
- require visible pairing and incoming-file approval by default; and
- avoid accounts, cloud relays, and background content uploads for normal
  operation.

It is a practical private workspace for the everyday problem of moving the
right file or message to the right nearby device—without making the internet a
mandatory middleman.

## What CrossDrop does

- Discovers nearby CrossDrop devices on the same private local network.
- Supports QR and code-based pairing when discovery is unavailable.
- Establishes a verified, encrypted connection before files or messages move.
- Lets the receiving person approve incoming files by default.
- Sends staged multi-file batches and small text or link messages.
- Keeps trusted-device information local to each device.
- Saves received files into an organised CrossDrop folder.

## Current platform support

| Platform | Status |
| --- | --- |
| Windows | Available as an internal signed installer. |
| Android | Available as a direct APK for early access. |
| macOS, iPhone/iPad, Linux | Planned; not yet distributed. |

## Product tour

The following approved screenshots show CrossDrop's current early-access
experience. They demonstrate the product flow only; actual nearby devices,
activity, and transfer history stay local to each person's devices.

### Windows

| Device directory | Secure device workspace | Incoming approval |
| --- | --- | --- |
| ![Windows device directory](assets/screenshots/Home%20Screen.png) | ![Windows secure device workspace](assets/screenshots/Device%20Workspace.png) | ![Windows incoming approval request](assets/screenshots/Approval%20Request.png) | | ![ About Crossdrop. Created by Dushyant Gadewal - #AskDushyant](assets/screenshots/About%20Crossdrop.png) |
| Find trusted or nearby devices and open a workspace. | Stage files or send a short secure message in one workspace. | Review an incoming transfer before accepting it. |

<p align="center">
  <img src="assets/screenshots/About%20Crossdrop.png" alt="About CrossDrop on Windows" width="720" />
</p>

<p align="center"><em>About CrossDrop: the privacy-first purpose and creator identity behind the product.</em></p>

### Android

| Device directory | Secure device workspace | Activity centre |
| --- | --- | --- |
| ![Android device directory](assets/screenshots/Mobile%20Home%20Screen.jpg) | ![Android secure device workspace](assets/screenshots/Mobile%20Device%20Workspace.jpg) | ![Android activity centre](assets/screenshots/Mobile%20Message%20Center.jpg) |
| Discover nearby devices or pair by QR code. | Switch between chat and staged files in a touch-first workspace. | Review device activity and incoming requests in one place. |

See the [screenshot index](assets/screenshots/README.md) for the purpose of
each image and public-release review guidance.

## Start here

1. Read [Getting started](docs/GETTING_STARTED.md).
2. Review [Privacy](docs/PRIVACY.md) and [Security](docs/SECURITY.md).
3. Download a release only from this repository's official **Releases** page
   once it is published.
4. Verify the release checksum before installing if you received a file
   outside GitHub.

## Current early-access builds

The current Android early-access build is `1.0.41+43`, validating local Windows
↔ Android transfers, trusted pairing, files, batches, messages, Android request
notifications while the phone is minimized or locked, and aligned CrossDrop
launcher branding. The current Windows installer is `1.0.42`, including the
responsive multi-device grid correction.

See [release notes](docs/RELEASES.md) for exact package names, checksums, and
known distribution limitations.

## Help and feedback

Use the repository's issue tracker for setup questions, usability feedback,
and reproducible non-sensitive problems. Do not include file contents,
verification codes, device identities, local IP addresses, or screenshots of
private data in a public issue.

For responsible vulnerability reporting, follow the instructions in
[SECURITY.md](SECURITY.md).

## Legal

CrossDrop is distributed under the binary-use terms in
[LICENSE-EULA.md](LICENSE-EULA.md). It is not an open-source release.

---

Created by **Dushyant Gadewal — #AskDushyant**.
