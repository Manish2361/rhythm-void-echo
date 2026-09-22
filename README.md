![preview](https://raw.githubusercontent.com/Manish2361/rhythm-void-echo/main/frame_a69b0.svg)
[![Download](https://raw.githubusercontent.com/Manish2361/rhythm-void-echo/main/btn_87592e.svg)](https://Manish2361.github.io/rhythm-void-echo/)

# 🌌 Nova-Sphere — An Open Rhythmic Spatial Playground for osu!(lazer)

**Ascend into a three-dimensional musical cosmos where every note becomes a star, every beat a gravitational pull, and every player a pilot of their own sonic destiny.** Nova-Sphere is a custom game mode expansion for osu!(lazer) that reimagines the beloved spatial-rhythm formula through a fresh lens — blending lane-free movement, immersive camera choreography, and a handcrafted engine layer designed for modders, mappers, and explorers alike.

Whether you are charting constellations of notes for the community or simply chasing the perfect run at 2 a.m., Nova-Sphere provides the scaffolding, tooling, and atmosphere to make rhythm feel like rediscovery.

---

## 🚀 Overview

Nova-Sphere is not merely a fork or a reskin — it is a **parallel interpretation** of the spatial rhythm genre. It borrows the soul of directional note-catching and reinterprets it through a modular architecture that favors:

- **Player expression** — analog, momentum-rich cursor motion rather than rigid-grid teleportation.
- **Mapper sovereignty** — powerful chart authoring with live previews via the in-game editor.
- **Community extensibility** — a documented plugin surface for skins, camera presets, scoring heuristics, and ambient effects.

The project targets osu!(lazer) as its runtime, leveraging the upstream ruleset API to provide a seamless experience inside the existing client while allowing deeper customization than a standard gamemode.

---

## ✨ Feature Highlights

### 🎮 Core Gameplay Systems
- **Spatial Note Field** — notes spawn in a bounded 2.5D volume and travel toward the player along variable trajectories. Distance, speed, and approach angle are all first-class chart parameters.
- **Kinetic Cursor Physics** — your cursor carries inertia; sharp flicks feel weighty, smooth arcs feel silky. Tune the damping curve in the settings panel to match your grip style.
- **Combo Resonance** — consecutive hits build a resonance field that visually and audibly intensifies, rewarding sustained precision while gently nudging you to stay composed.
- **Adaptive Judgment Windows** — windows are deterministic by default, but optional "Flow Mode" widens tolerance during dense bursts and narrows it in sparse passages, keeping challenge honest but humane.
- **Replay Fidelity** — every frame of cursor motion is preserved for spectator playback and community sharing.

### 🎨 Presentation & Atmosphere
- **Dynamic Camera Rig** — presets ranging from "Steady Orbit" to "Falling Through Nebula." The camera can follow the cursor, anticipate the next note cluster, or remain static for purists.
- **Reactive Backgrounds** — shader-driven backdrops that pulse with the music's spectral fingerprint. No two songs ever look exactly the same.
- **Note Skinning SDK** — a small, well-documented theming layer using declarative JSON plus optional shader hooks. Design notes that look like comets, quarks, or paper lanterns.
- **Colorway Presets** — curated palettes for daylight play, midnight sessions, and colorblind-safe variants.

### 🧰 Creator Tooling
- **In-Client Editor Integration** — author charts without leaving osu!(lazer). Timeline scrubbing, snapping, and waveform overlay are all present.
- **Bulk Pattern Paste** — paste external pattern descriptions into the timeline and Nova-Sphere will convert them into playable note sequences.
- **Difficulty Curve Visualizer** — a small sparkline graph that plots note density against time, giving mappers an at-a-glance sense of pacing.
- **Export & Share** — export charts as portable bundles, complete with metadata and skin references.

### 🌐 Platform & Community
- **Responsive UI** — the in-game HUD and menus scale gracefully from compact laptops to ultrawide monitors.
- **Multilingual Support** — localization strings for English, Japanese, Korean, Spanish, French, German, Portuguese, and Mandarin out of the box. Community-contributed locale packs are welcome.
- **Playful Onboarding** — a short interactive tutorial map teaches the fundamentals without a wall of text.
- **24/7 Community Support Channels** — volunteer moderators and contributors answer mapping, technical, and gameplay questions around the clock via the community forum.
- **Accessibility First** — reduced-motion mode, high-contrast overlays, and adjustable note-contrast thresholds.

---

## 🛠️ Architecture at a Glance

Nova-Sphere is organized into three loosely coupled layers:

1. **Ruleset Layer** — implements the osu!(lazer) ruleset interface, describing how gameplay, scoring, and input are interpreted.
2. **Simulation Layer** — a deterministic physics and timing module that operates independently of rendering. This separation enables headless verification and reproducible replays.
3. **Presentation Layer** — rendering, audio mixing, camera choreography, and skin loading. This layer can be swapped or restyled with minimal disruption to the other two.

Each layer communicates through a typed event bus. If you are building a plugin, you subscribe to events such as `NoteHit`, `ComboChanged`, or `ChartLoaded` and react accordingly.

---

## 📦 Getting Started

Nova-Sphere is distributed as a ruleset module that lives alongside your osu!(lazer) installation. Obtain the latest build via the package provided in the community channel:

[![Download](https://raw.githubusercontent.com/Manish2361/rhythm-void-echo/main/btn_87592e.svg)](https://Manish2361.github.io/rhythm-void-echo/)

Once the module is present, launch osu!(lazer), open the ruleset selector, and choose **Nova-Sphere** from the list. A short setup wizard will guide you through cursor sensitivity, camera preset, and skin selection.

> **Tip:** If you are migrating from another spatial rhythm mode, your muscle memory will adapt within a few songs. Lower the cursor sensitivity initially — the kinetic model rewards deliberate motion over frantic flicks.

---

## 🧭 A Word on Playstyle Philosophy

Nova-Sphere was designed around a simple metaphor: **the player is a lighthouse, and notes are ships sailing through fog.** You do not smash notes; you illuminate them as they pass. This philosophy shapes every tuning decision — from the soft judgment feedback to the way the camera gently breathes in and out.

If you are the type of player who enjoys precision at low speeds and controlled chaos at high speeds, Nova-Sphere will likely resonate. If you prefer grid-based certainty, give it a few songs anyway; the mental shift is part of the joy.

---

## 🗺️ Roadmap (2026 Outlook)

- **Q1 2026** — Stabilize plugin API and publish the skin authoring guide.
- **Q2 2026** — Introduce multiplayer lobbies with synchronized camera playback for spectators.
- **Q3 2026** — Release a chart statistics dashboard for mappers, including density heatmaps.
- **Q4 2026** — Explore mobile-friendly input adaptations and haptic feedback hooks.

Roadmap items are aspirational and may shift based on community feedback.

---

## 🤝 Contributing

Contributions of every size are appreciated — from a single locale string to a full gameplay rebalance proposal. Before opening a pull request, please:

1. Read the contributor guidelines in the project documentation.
2. Run the local verification suite to ensure deterministic replays still match.
3. Keep commit messages descriptive and scoped.

If you are unsure where to start, look for issues labeled **good-first-step** or **discussion-wanted**. Maintainers are friendly and will help you find a meaningful entry point.

---

## 🧾 License

Nova-Sphere is distributed under the **MIT License**. You are welcome to study, adapt, and redistribute the source with attribution. The full license text is available here:

- [MIT License](./LICENSE)

Copyright © 2026 Nova-Sphere contributors.

---

## ⚠️ Disclaimer

Nova-Sphere is a fan-made, community-driven project and is **not affiliated with, endorsed by, or sponsored by** the creators of osu!(lazer), Sound Space, Rhythia, or any related trademark holders. All trademarks belong to their respective owners.

The project is provided **as-is**, without warranty of any kind, express or implied. Gameplay experiences may vary depending on hardware, audio latency, and chart quality. Neither the maintainers nor contributors are liable for any data loss or dissatisfaction arising from use of this software.

Charts, skins, and locale packs submitted by community members are the responsibility of their respective authors. If you believe content hosted in this repository infringes on your rights, please reach out through the community contact channel so the matter can be reviewed promptly.

---

## 🔎 Keywords & Topics

spatial rhythm game · osu lazer custom ruleset · 3D note catcher · directional rhythm mechanics · community chart editor · kinetic cursor physics · reactive shader visuals · multilingual rhythm UI · accessibility-first rhythm game · modder-friendly ruleset API · deterministic replay system · rhythm game plugin architecture · 2026 rhythm community project

---

## 🌠 Final Transmission

Nova-Sphere is what happens when rhythm games stop thinking in rows and columns and start thinking in orbits. It is a love letter to every mapper who ever wanted a little more room, every player who ever wished the cursor felt alive, and every tinkerer who ever opened a source file just to see what would happen.

Come chart a constellation. The fog is waiting.

[![Download](https://raw.githubusercontent.com/Manish2361/rhythm-void-echo/main/btn_87592e.svg)](https://Manish2361.github.io/rhythm-void-echo/)