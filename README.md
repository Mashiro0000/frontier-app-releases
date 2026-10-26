# Frontier App releases

This repository holds only the signed installers of Frontier App and the `latest.json` file the app reads to find an update. It contains no source code.

Every `latest.json` is signed with the owner's release key. An installed Frontier App accepts an update only when that signature is valid and the installer's SHA-256 matches the one it names, so a file placed here by anyone else is refused.

To check an installer by hand before a first install: `Get-FileHash frontier-app-<version>-setup.exe` and compare it with the SHA-256 in that release's notes.
