# Security Policy

## Our security approach

CrossDrop is built for direct local transfers. Devices discover one another on
the local network, then establish an encrypted session before messages or files
move. A person confirms a pairing code for a new connection, and incoming files
require approval by default.

CrossDrop does not claim to replace a managed corporate security system,
endpoint protection, or a secure backup strategy.

## Supported release line

Only the newest release published on the official GitHub Releases page is
considered supported for security fixes. Early-access releases may be retired
when a corrective update is available.

## Reporting a vulnerability

Please do **not** report security issues in a public GitHub issue.

Until GitHub private vulnerability reporting is enabled for the public
repository, contact the repository owner privately through GitHub and include:

- the CrossDrop version and platform;
- clear reproduction steps;
- the observed and expected result; and
- a safe proof of concept, if available.

Do not send private files, passwords, pairing codes, full device identities,
or local-network credentials.

After the repository is created, the maintainer should enable GitHub's
**Private vulnerability reporting** and replace this paragraph with its direct
reporting link.

## Security boundaries

- CrossDrop protects data in transit between participating devices; it cannot
  protect a device that is already compromised.
- A person must confirm a new pairing before trusting a device identity.
- Trusted-device automatic file receipt is off by default and remains limited
  to the selected trusted identity and its configured size limit.
- Android system notifications intentionally avoid exposing verification codes
  or message content.
- CrossDrop is designed for private local networks. Treat unknown public or
  shared Wi-Fi networks with additional caution.

## Security updates

If a release is marked security-critical, install it promptly on every device
that participates in the same CrossDrop workspace. Review the corresponding
release notes before updating.
