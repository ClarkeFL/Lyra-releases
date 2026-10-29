# Lyra downloads

Binaries only. This repo exists so Lyra's in-app updater and the installer can
fetch releases without a GitHub login; the source lives in a private repo.

## Install (Apple Silicon)

```sh
curl -fsSL https://github.com/ClarkeFL/Lyra-releases/releases/latest/download/install.sh | sh
```

No Gatekeeper prompt: `curl` doesn't set the `com.apple.quarantine` flag that
invokes it. The app updates itself from here after that.

### DMG instead

Grab `Lyra_x.y.z_aarch64.dmg` from [Releases](../../releases/latest) and drag
Lyra to Applications. The build is signed with a self-signed certificate, so
the first launch needs right-click, Open.

Lyra needs the [Claude Code](https://docs.claude.com/en/docs/claude-code) CLI
installed and logged in.
