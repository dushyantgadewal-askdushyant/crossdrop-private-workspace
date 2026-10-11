# GitHub Publishing Runbook

This runbook publishes only the source-free public package. It must never be
run from the CrossDrop repository root.

## Publication target

- **Owner:** `dushyantgadewal-askdushyant`
- **Repository:** `crossdrop-private-workspace`
- **Visibility:** Public
- **Repository purpose:** Product documentation, approved screenshots, release
  notes, and approved distribution material only. No CrossDrop source code,
  internal documentation, signing certificate material, private Git history,
  or build tooling is included.

## Pre-flight review

1. Confirm GitHub is connected to the intended owner account.
2. Re-read `SOURCE_FREE.md` and `assets/screenshots/README.md`.
3. Confirm that the approved screenshots contain no unapproved private device
   labels, IP addresses, QR/pairing codes, message content, local paths, or
   file names.
4. Create the repository as a new empty public repository with no generated
   README, licence, or `.gitignore` file.

## Exact local commands

Run the following only after GitHub account access has been confirmed. They
create a separate Git history inside `public_release`, so the parent CrossDrop
repository and its private source are never selected for upload.

```powershell
Set-Location 'E:\Development-AI-Projects\CrossDrop\public_release'
git init --initial-branch=main
git add --all
git status --short
git commit -m 'Publish CrossDrop private workspace product home'
git remote add origin 'https://github.com/dushyantgadewal-askdushyant/crossdrop-private-workspace.git'
git push -u origin main
```

## Verification commands

```powershell
git remote -v
git status --short
git log -1 --oneline
```

Then open the repository in a browser and confirm that the README product tour
renders all six screenshots and that source code, installer files, signing
assets, and internal documentation are absent.

## Execution record

| Date | Action | Result |
| --- | --- | --- |
| 2026-10-11 | GitHub API: list connected accounts | No account was returned to this workspace, so no repository was created and no files were uploaded. |
| 2026-10-11 | `gh auth status` | GitHub CLI is not installed on this Windows profile. No installation was attempted and no external change was made. |
| 2026-10-11 | `git ls-remote --heads https://github.com/dushyantgadewal-askdushyant/crossdrop-private-workspace.git` | Confirmed the newly created public repository is reachable and empty. |
| 2026-10-11 | `git init --initial-branch=main` | Created an isolated Git repository inside `public_release` only. |
| 2026-10-11 | `git config user.name 'Dushyant Gadewal - #AskDushyant'` | Set the author for the isolated public repository. |
| 2026-10-11 | `git config user.email 'dushyant.gadewal@blackdemon.in'` | Set the author email for the isolated public repository. |
| 2026-10-11 | `git add --all` | Staged only source-free public documentation and approved assets from `public_release`. |

## Current blocker

The GitHub connector currently has no accessible account in this workspace, and
the local GitHub CLI is not installed. Reconnect or authorize the GitHub
integration for `dushyantgadewal-askdushyant`, then repeat the pre-flight review
before running the commands above. Installing the GitHub CLI is optional and
must be explicitly approved; it is not required when the connector is properly
authorized.

