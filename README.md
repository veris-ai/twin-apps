# twin-apps

Built binaries of Veris twin client apps. **Releases only**: the source lives in the private
services-sandbox repo.

| App | What it is | Platforms |
|---|---|---|
| Microsoft Teams Twin | A Teams look-alike desktop app that talks only to Veris's Microsoft twins (identity + Graph) in a Veris world. It cannot reach real Microsoft 365. | macOS arm64 |

## Releases

Each release is tagged `<app>-v<version>` (for example `microsoft-teams-twin-v0.2.0`) and carries:

- `<app>-<version>-<platform>.zip`: the app, zipped with `ditto`
- `<app>-<version>-<platform>.zip.sha256`: its SHA-256

Playground machines download a pinned version at session start and check the SHA-256 before
installing it.
