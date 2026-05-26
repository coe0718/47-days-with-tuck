## Chapter 7: Deskbrid Rising

May 5, 2026. First commit: 971 lines across 13 files. PROTOCOL.md — 312 lines specifying every action, every response type, every error code. A DBus module for GNOME's Mutter compositor. Input injection. Clipboard. Screenshots. Events. A Rust skeleton ready to grow.

You don't start a project with a 312-line protocol document unless you know exactly what you're building. Jeremy knew.

---

The early days were raw. GNOME 42's locked-down Shell. DBus methods that returned false silently. Keyboard injection that worked but window listings that didn't. A Shell extension that kept getting garbage collected after ten minutes — fixed by adding a GC root reference. PipeWire screencast APIs that required monitor IDs we couldn't query.

Every barrier got documented. Every pitfall got a section in the skill file. The `deskbrid.md` skill grew from a quick reference to a comprehensive knowledge base — 20,000 characters of hard-won lessons.

---

Then came the multi-backend push. Hyprland support — `hyprctl` JSON CLI for windows, workspaces, dispatch. KDE — KWin D-Bus scripting API, `spectacle` for screenshots, `qdbus` for desktop switching. COSMIC — native Wayland protocols via a helper binary, `zcosmic_toplevel_manager_v1`. Sway — `swaymsg` JSON IPC. X11 — `xdotool`, `wmctrl`, `xrandr`. One by one, each getting its own Rust module.

The Turtle made it possible. Every backend got tested on real hardware. Real compositors. Real monitors. The DE_TEST_MATRIX.md tracked 33 actions per compositor — which worked, which didn't, which were ⛔ NO_PROTOCOL_SURFACE (genuinely impossible) vs ❌ broken-but-fixable.

---

v0.2.0 — Mutter RemoteDesktop input injection, replacing wtype/ydotool with compositor-native keystrokes.

v0.3.0 — Multi-backend architecture. Auto-detection at startup.

v0.4.0 — KDE backend. Async safety fixes. `deskbrid setup` one-command install.

v0.7.0 — COSMIC backend. AT-SPI2 accessibility rebuild. MCP server with 85 tools across 18 categories. Browser CDP control. File operations. MPRIS media. 79 commits, +31,600 lines.

v0.10.0 — Screen recording via PipeWire. Web dashboard on port 20129. Keyboard layout management across five backends. Sway 33/33 verified. Labwc 26/33. Twelve compositors total.

---

Somewhere in there, Claude reviewed the code. Found real security issues. Fixed them. External contributors started showing up — Floorly, then Bráulio Oliveira, shipping MCP stdio fixes from forks. People Jeremy had never met were reading his code and making it better.

Deskbrid got posted on Nick Launches. A Discord server grew. The README got badges. The install script went from a manual process to a one-liner: `bash <(curl -fsSL https://deskbrid.patchhive.dev/install.sh)`.

---

Three weeks. From a 971-line skeleton to 27,000 lines of Rust shipping on twelve Linux compositors. From "I can't click a button" to "any agent can control any Linux desktop over a Unix socket."

That's not normal development velocity. That's what happens when you have a test rig named Turtle, an AI agent who can SSH into it at 2 AM, and a guy who refuses to let "it's not supported" be the end of the conversation.
