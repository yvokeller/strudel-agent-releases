# Strudel for macOS

Releases of **Strudel for macOS**, the Mac app of Strudel, a personal AI assistant framework: the
Strudel web UI in a window, an overlay on a global shortcut (ask an agent from any app, push-to-talk),
calls with your agents, notifications and a share menu. It connects to your own
Strudel server (for example over Tailscale); the app alone does nothing.

The source code is private; this repository only hosts the signed builds and the update feed.

## Download

**[Download the latest Strudel.dmg](https://github.com/yvokeller/strudel-agent-releases/releases/latest/download/Strudel.dmg)**
(all versions: [Releases](https://github.com/yvokeller/strudel-agent-releases/releases)).

Open the DMG and drag Strudel to Applications. Requires macOS 26 or later.
The app is signed with a Developer ID and notarized by Apple.

## Updates

Strudel updates itself with [Sparkle](https://sparkle-project.org): it checks once a day (and on
*Strudel → Check for Updates…* or in the menu bar menu), shows what is new and installs the new version
when you agree. Every update is notarized and signed with an EdDSA key whose public half is built into
the app, so only builds from the release machine are accepted.

- Update feed: [`appcast.xml`](https://raw.githubusercontent.com/yvokeller/strudel-agent-releases/main/appcast.xml) (generated from [`releases.json`](releases.json))
- Turn automatic checks off in Strudel's settings (*Updates*).
