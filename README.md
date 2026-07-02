# Ascertainty FC

**A playable football match built around the [Ascertainty](https://ascertainty.xyz) thesis** — the players were commissioned, AI-built, verified, and settled on-chain *off the pitch*, then fielded.

Built in **Unreal Engine 5.8**. Grab a player, dribble up the pitch, and score.

---

## Play

- **▶ Play now (Windows):** **[grain-by-grain.itch.io/ascertainty-fc](https://grain-by-grain.itch.io/ascertainty-fc)**
- **Or open the project** in Unreal Engine 5.8 — see below.

## Controls

| Input | Action |
|---|---|
| **W A S D** / Arrows | Move |
| **Left Shift** (hold) | Sprint — drains the stamina bar |
| **Left Mouse** (hold → release) | Shoot / kick — hold to charge power |
| **Right Mouse** | Pass |
| **E** | Tackle |
| **Spacebar** | Jump |

Get near the opponent goal and shoot — a goal-magnet assist curves the ball into the net.

## Open it in the editor

This is a **Blueprint-only** project — no C++ compile step.

1. Install **Unreal Engine 5.8** via the Epic Games Launcher.
2. Install **Git LFS** and run `git lfs install` once per machine, then clone this repo.
3. Open `Football.uproject` and press **Play**. The default map (`Lvl_Match`) loads a 1‑v‑9 match on a walled pitch.

The match plays on a simple pitch out of the box. For the finished look — the AI‑built footballer model and the stadium shell — add the two Fab packs below (optional).

### Optional: the Fab visual packs

These are **Fab Standard License** packs. They can ship *inside* a built game, but the license doesn't allow redistributing them as source, so they're excluded here. **Without them the match still plays** (players fall back to default meshes and there's no stadium). For the full look, buy each on [Fab](https://www.fab.com) and drop it into `/Content`:

| Pack | Adds | Destination |
|---|---|---|
| **White_Football_Player** (Code This Lab) | the footballer model | `Content/White_Football_Player/` |
| **Statium_Soccer** | the stadium shell | `Content/Statium_Soccer/` |

## The idea

Each player was commissioned to a spec → produced by an AI swarm → **verified by Grain** (rig + geometry + textures) → **settled on-chain** → then fielded. That pipeline runs *off-screen*; the game itself is just the match on the pitch.

## License

Original Ascertainty FC content (the `Content/Ascertainty` assets and project config): **MIT** (see [`LICENSE`](LICENSE)).

Redistributed Unreal Engine template content (`Content/Characters`, `Content/LevelPrototyping`, `Content/Football`, `Content/ThirdPerson`, `Content/Input`) is provided under the **Unreal Engine EULA** — usable only within Unreal Engine projects, not covered by MIT.

Third-party Fab packs (above) are **not** included and remain governed by their own licenses.
