<div align="center">
  <img src="assets/logo.png" alt="Elden Trials logo" width="124" />

  <h1>ELDEN TRIALS</h1>

  <p><strong>Master the battle. Claim your place.</strong></p>
  <p>Competitive boss time trials for <strong>Elden Ring</strong>.<br />
  Fixed builds. Real arenas. One clock.</p>

  <p>
    <a href="https://github.com/foxday/elden-trials-releases/releases/latest"><img src="https://img.shields.io/github/v/release/foxday/elden-trials-releases?label=Latest%20release&color=c9a86a&style=flat-square" alt="Latest release" /></a>
    <img src="https://img.shields.io/badge/Platform-Windows-555555?style=flat-square" alt="Windows" />
    <img src="https://img.shields.io/badge/Status-Beta-d08a3c?style=flat-square" alt="Beta" />
  </p>

  <p>
    <strong><a href="https://github.com/foxday/elden-trials-releases/releases/latest">Download</a></strong> ·
    <a href="https://eldentrials.org">Website</a> ·
    <a href="https://eldentrials.org/leaderboards">Leaderboards</a> ·
    <a href="https://www.nexusmods.com/eldenring/mods/11468">Nexus Mods</a>
  </p>
</div>

---

## What is Elden Trials?

**Elden Trials** turns Elden Ring boss fights into competitive time trials. Every challenge gives you a **predefined build** and puts you directly into the boss arena. No farming, no leveling, no equipment advantage: just learn the build and beat the clock.

Your best times compete on online leaderboards, from individual bosses to cumulative global and seasonal rankings.

### Features

- **Handcrafted boss challenges** — Fixed weapons, stats and equipment for each fight.
- **Normal & No Hit** — Two modes with separate leaderboards.
- **World leaderboards** — Chase personal bests, world records and your rank in each challenge.
- **Global & seasonal competition** — Track progress across challenges, not just individual fights.
- **Achievements & player profiles** — Keep track of your clears and records.
- **Community Beta Trials** — Beta testers can submit challenges for other testers to try and review.

## Download & install

**[Download the latest Elden Trials release](https://github.com/foxday/elden-trials-releases/releases/latest)**

1. Download `EldenTrials-<version>.zip` from the latest release.
2. Extract the ZIP to a writable folder, such as `C:\Games\EldenTrials`. **Do not** extract it into the Elden Ring installation folder.
3. Run `EldenTrials.exe` and complete the initial setup.
4. Press **Play** to launch Elden Ring with the mod and dedicated save.

**Mod Engine 3 is included.** You do not need to install it, .NET or Visual C++ runtimes separately.

## How to play

1. Launch the game using **`EldenTrials.exe`**.
2. Choose **Continue** or **Load Game**, and enter with the dedicated **`elden_trials`** character.
3. Go to **Roundtable Hold**, rest at the grace and select **Elden Trials**.
4. Choose **Normal** or **No Hit**, select a challenge and press **START**.
5. Defeat the boss. If you've registered a player account, your result is submitted automatically.

## Before you play

> [!IMPORTANT]
> **Offline only.** The launcher starts Elden Ring with Easy Anti-Cheat disabled. Online play is not supported; no manual EAC changes are required.
>
> **Your main save is not touched.** Elden Trials uses its own dedicated `elden_trials` save. Your existing characters are not loaded, edited or replaced by the mod.

**Requirements:** Windows 10/11 (64-bit), **Elden Ring + Shadow of the Erdtree**, and a game executable matching the supported **regulation 1.17.1** build. The Tarnished Edition is supported if it includes the expansion.

> [!NOTE]
> Elden Trials is currently in **beta**. Challenges and balance may change, and progress resets are possible between builds.

## Updates

The launcher checks for new versions through GitHub Releases and can update itself. Challenge content can also be delivered through the remote catalog without reinstalling the mod.

<details>
<summary><strong>Setup, accounts & Steam detection</strong></summary>

### Steam detection

- **Steam detected:** The launcher locates the game and save folder automatically. Keep Steam running while playing.
- **Steam not detected:** Select `eldenring.exe` and the destination for the dedicated save manually.

Both setups use the same separate `elden_trials` save.

### Player account

- Your account, token and launcher settings are stored under `%APPDATA%\EldenTrials`.
- When creating an account, **save the recovery code** displayed during registration. It is needed to recover the account on another PC.
- Leaving the player name blank launches the game without a leaderboard account.
- If an existing player is recognized through Steam, the launcher can restore that player's progress.

### Windows SmartScreen

The launcher is not code-signed, so Windows may show a SmartScreen warning. Only run files you've obtained from this project's official GitHub release and verified as trustworthy.

</details>

<details>
<summary><strong>Updating from older versions</strong></summary>

- Installations **older than v0.5.0** require a manual upgrade to v0.5.0 or newer before automatic updates can work.
- The updater verifies the downloaded ZIP using SHA-256, creates a backup and preserves the `config` and `dist` folders during the update process.
- Player account data is stored outside the mod folder, in `%APPDATA%\EldenTrials`.

</details>

<details>
<summary><strong>Troubleshooting & logs</strong></summary>

| Problem | What to try |
| --- | --- |
| Steam isn't detected | Select `eldenring.exe` and the dedicated-save destination manually. |
| The game won't launch with Steam installed | Start Steam, then launch `EldenTrials.exe` again. |
| The game opens without the mod | Use `EldenTrials.exe`, not the game's normal launcher. |
| Unsupported game build | Check that your executable matches the supported 1.17.1 build. |
| The `elden_trials` character is missing | Verify the save folder selected during setup. |
| Antivirus quarantines a file | Confirm that the ZIP came from the official release and inspect the detection before making any security exception. |
| The overlay or selector doesn't appear | Close the game and inspect the logs below. |
| You lost access to your account | Use your saved recovery code. Without it, the account cannot be recovered. |

**Log locations**

```text
dist\equipment-runtime\equipment.log
dist\equipment-runtime\cards-overlay.log
```

For help, [open an issue](https://github.com/foxday/elden-trials-releases/issues) or contact [teruelpablo@gmail.com](mailto:teruelpablo@gmail.com). Include the steps to reproduce, expected and actual behavior, and any relevant logs or screenshots.

</details>

<details>
<summary><strong>Uninstall</strong></summary>

1. Close Elden Ring and the launcher.
2. Delete the Elden Trials installation folder.
3. Optionally delete `%APPDATA%\EldenTrials` to remove local account credentials and settings.

Uninstalling does not modify your main Elden Ring save.

</details>

---

### Credits

**PHT** — Design, development and challenge creation.

Built with **Mod Engine 3** (garyttierney; MIT / Apache-2.0), **Dear ImGui** (ocornut) and **MinHook** (TsudaKageyu). Fonts: **Cinzel**, **Inter** and **Gelasio** (SIL OFL 1.1). Icons: **Font Awesome Free** (CC BY 4.0 / SIL OFL 1.1).

<sub>**Disclaimer:** Elden Trials is an unofficial community project and is not affiliated with or endorsed by FromSoftware or Bandai Namco Entertainment. Elden Ring and Shadow of the Erdtree are trademarks of their respective owners.</sub>

<div align="center">
  <sub>Made by PHT · <a href="mailto:teruelpablo@gmail.com">Contact</a></sub>
</div>
