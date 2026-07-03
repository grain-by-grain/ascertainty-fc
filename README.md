# Ascertainty FC
<img width="1280" height="720" alt="splash-screen" src="https://github.com/user-attachments/assets/0d0e1ba5-abe2-478e-9ab2-3967b623f6f8" />

**A playable football match built around the [Ascertainty](https://ascertainty.com) thesis** — the players were commissioned, AI-built, verified, and settled on-chain *off the pitch*, then fielded.

Built in **Unreal Engine 5.8**. Grab a player, dribble up the pitch, and score.

---

## Play

**Two ways in:**

**1 · Download & play (Windows) — no setup.**
Grab the packaged build — the player model, stadium, and every mechanic are baked in. Unzip and run.
▶ **[grain-by-grain.itch.io/ascertainty-fc](https://grain-by-grain.itch.io/ascertainty-fc)**

**2 · Clone & open in Unreal Engine 5.8 — for builders.**
Build it yourself and field your own players. See *Open it in the editor* below.

## Controls

| Input | Action |
|---|---|
| **W A S D** / Arrows | Move |
| **Left Shift** (hold, or double-tap) | Run / sprint — drains the stamina + sprint bars |
| **Left Mouse** (hold → release) | Shoot / kick — hold to charge power |
| **Right Mouse** | Trap the ball / pass to a teammate |
| **E** | Tackle |
| **Spacebar** | Jump |

Get near the opponent goal and shoot — a goal-magnet assist curves the ball into the net. The mini-map (bottom-right) shows opponents (red), teammates (blue), and the ball (yellow).

## Open it in the editor

This is a **Blueprint-only** project — no C++ compile step.

1. Install **Unreal Engine 5.8** (Epic Games Launcher).
2. Install **Git LFS**, run `git lfs install` once, then clone this repo.
3. Open `Football.uproject` and press **Play** — the default map (`Lvl_Match`) loads a match with AI teammates and opponents on a walled pitch.

**Every mechanic works out of the box** on a placeholder pitch. The player model and stadium are **not** in this repo (licensing) — so you bring your own.

### Bring your own 3D assets — the Ascertainty way

This project deliberately ships with **no character or stadium art**. That's the point: field players *you* trust. Supply your own — and for the full Ascertainty treatment, have them **verified by Grain** before you put them on the pitch:

- **Generate & verify** — commission or AI-generate a footballer (or stadium), then run it through **Grain's verification** — rig, geometry, textures — with an optional **on-chain settlement** as proof. Start at **[grainbygrain.xyz](https://grainbygrain.xyz)**.
- **Purchase & verify** — buy a compatible pack and put it through the same check. The demo uses two **Fab Standard License** packs; grab them on [Fab](https://www.fab.com) for the exact look in the video.

Drop whatever you field into these folders:

| Asset | Adds | Destination |
|---|---|---|
| Player model *(demo uses White_Football_Player, Code This Lab)* | the footballer | `Content/White_Football_Player/` |
| Stadium *(demo uses Statium_Soccer)* | the arena | `Content/Statium_Soccer/` |

Without them the match still plays — players fall back to default meshes and there's no stadium.

## The idea

Each player was commissioned to a spec → produced by an AI swarm → **verified by Grain** (rig + geometry + textures) → **settled on-chain** → then fielded. That pipeline runs *off-screen*; the game itself is just the match on the pitch. Learn more at **[grainbygrain.xyz](https://grainbygrain.xyz)**.

## License

Original Ascertainty FC content (the `Content/Ascertainty` assets and project config): **MIT** (see [`LICENSE`](LICENSE)).

Redistributed Unreal Engine template content (`Content/Characters`, `Content/LevelPrototyping`, `Content/Football`, `Content/ThirdPerson`, `Content/Input`) is provided under the **Unreal Engine EULA** — usable only within Unreal Engine projects, not covered by MIT.

Third-party Fab packs (above) are **not** included and remain governed by their own licenses.
