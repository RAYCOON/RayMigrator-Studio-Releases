# RayMigrator Studio — Releases

Download page for RayMigrator Studio, the management interface for the
RayMigrator database migration engine. This repository holds only the release
archives; see [Releases](https://github.com/RAYCOON/RayMigrator-Studio-Releases/releases).

## Downloads

Each release has one archive per platform:

| Platform | Archive |
| :- | :- |
| Windows x64 | `RayMigrator-Studio-<version>-win-x64.zip` |
| macOS Apple Silicon | `RayMigrator-Studio-<version>-osx-arm64.tar.gz` |
| Linux x64 | `RayMigrator-Studio-<version>-linux-x64.tar.gz` |

Each archive holds the server `raymigrator-studio` with the web interface, the
CLI `RayMigrator-Management` and `THIRD-PARTY-NOTICES.md`.

## Requirements

- The [ASP.NET Core Runtime 10.0](https://dotnet.microsoft.com/download/dotnet/10.0)
  (or the .NET 10 SDK). The plain .NET Runtime is not enough.

## Getting started

1. Unpack the archive.
2. macOS: the binaries are not notarized. In the extracted folder, run
   `xattr -d com.apple.quarantine raymigrator-studio RayMigrator-Management`
   before the first start.
3. Windows: the executables are not signed. If SmartScreen warns, choose
   "More info" and "Run anyway".
4. Start `raymigrator-studio`. It listens on 127.0.0.1 and opens the browser
   with a start token.

The first start of a build unpacks it into `~/.net/raymigrator-studio/<bundle id>/`
(Windows `%TEMP%\.net\raymigrator-studio\<bundle id>\`).

## Licence

Licence terms are pending; until they are published, contact
RAYCOON.com GmbH for the terms of use.
