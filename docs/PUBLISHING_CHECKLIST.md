# Public GitHub Publishing Checklist

Use this checklist after approving this package and before making a repository
or release public.

## Repository

- [ ] Create a new **public, documentation-only** repository, for example
      `crossdrop-private-workspace` under `dushyantgadewal-askdushyant`.
- [ ] Copy only the contents of `public_release/`; do not copy `app/`,
      `packages/`, internal `docs/`, build scripts, signing material, or the
      private Git history.
- [ ] Follow [the publishing runbook](GITHUB_PUBLISHING_RUNBOOK.md), which
      creates a separate Git history inside `public_release/` before pushing.
- [ ] Add the approved logo and product screenshots to `assets/`.
- [ ] Enable GitHub Issues for non-sensitive support feedback.
- [ ] Enable private vulnerability reporting before announcing the project.
- [ ] Review all public text for unwanted local paths, device names, IP
      addresses, test data, emails, or internal process details.

## First release

- [ ] Build fresh approved Android and Windows packages.
- [ ] Calculate SHA-256 checksums again and update `docs/RELEASES.md`.
- [ ] Attach only approved release assets to GitHub Releases.
- [ ] Add the release notes for the exact version.
- [ ] Test downloading each asset from a browser on a non-development device.
- [ ] Explain the Android APK installation step and current Windows
      self-signed-certificate warning honestly.

## Before broader distribution

- [ ] Obtain and apply a publicly trusted Windows code-signing certificate.
- [ ] Obtain legal review for `LICENSE-EULA.md` and `docs/PRIVACY.md`.
- [ ] Decide a real support and security-reporting contact route.
- [ ] Capture current Windows and Android screenshots with no personal device
      names, messages, files, QR codes, or network data visible.
- [ ] Re-test pairing, normal/batch files, messaging, offline handling,
      Android lock/minimize notifications, and a cancelled transfer.
