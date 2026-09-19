<div align="center">

<img src="https://raw.githubusercontent.com/ARK-tube/ARKtube/main/arktube_linux/resources/icons/appIcon.png" alt="ARKtube" width="296" height="296">

# ARKtube

**YouTube, as a native desktop app.**

Keep the UI. Keep the player. Change the shell.

</div>

---

## What we build

ARKtube wraps YouTube's own TV (Leanback) interface in a thin native shell, so it
behaves like an installed application instead of a browser tab. No redesign, no
replacement frontend, no bundled copy of the site. YouTube stays YouTube; we only
own the window around it.

```text
YouTube (youtube.com/tv)  +  GTK3 + WebKit2GTK  =  YouTube, installed.
```

## Projects

| Project | What it is | Where |
|---|---|---|
| **ARKtube for Linux** | Native GTK3 + WebKit2GTK client for `youtube.com/tv`: fullscreen persistence, gamepad and remote input, offline screen, boot splash, `.deb` builds from CI | [`main`](https://github.com/ARK-tube/ARKtube) |
| **Webtop** | A session layer that makes ARKtube selectable from the Ubuntu login screen, without starting the full GNOME Shell desktop | [`webtop`](https://github.com/ARK-tube/ARKtube/tree/webtop) |
| **Webtop, Sway edition** | The same idea on Sway: ARKtube is the only window the compositor ever shows, fullscreen and borderless | [`arktube-layer-shell`](https://github.com/ARK-tube/ARKtube/tree/arktube-layer-shell) |
| **ARKtube for Android** | A WebView shell around YouTube's mobile web UI | [`Android`](https://github.com/ARK-tube/ARKtube/tree/Android) |

## Design principles

- **Add the smallest layer that works.** If YouTube already solves a problem, we let it.
- **Own the window, not the page.** The native side handles window state, input mapping,
  and connectivity. The page is never re-implemented.
- **Stay small until the approach is proven.** Linux first; other platforms only after
  the Linux design holds up.

## Status

Early and in progress. The Linux app runs today; tray integration, Immersive Mode,
AppImage packaging, and non-Linux builds are not ported yet. The repository's
[roadmap](https://github.com/ARK-tube/ARKtube#status) tracks what is done and what is open.

## Try it

```bash
git clone https://github.com/ARK-tube/ARKtube.git
cd ARKtube/arktube_linux
cmake -B build -S . && cmake --build build
./build/arktube_linux
```

Requires CMake ≥ 3.16, a C11 compiler, `libgtk-3-dev`, and `libwebkit2gtk-4.1-dev`.
Full instructions are in the [repository README](https://github.com/ARK-tube/ARKtube#install).

---

<sub>ARKtube is an independent project. It is not affiliated with or endorsed by Google or YouTube.
YouTube is a trademark of Google LLC.</sub>
---

<sub>ARKtube is an independent project. It is not affiliated with or endorsed by Google or YouTube.
YouTube is a trademark of Google LLC.</sub>
