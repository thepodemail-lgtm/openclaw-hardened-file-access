# Security Policy

## Scope
The file-access skill reads, lists, and copies files only inside folders named in its allowlist. It never deletes, moves, or overwrites files, and it refuses credential and key files by design. Every run writes an audit log, and a run stopped by a cap closes the log with a PARTIAL marker.

## Reporting a vulnerability
Open a private report through GitHub's security advisory flow on this repository, or contact the maintainers via the repository owner. Please do not post exploit details in a public issue before a fix is available.

## Supported versions
Only the latest release on the main branch is supported.
