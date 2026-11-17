<div align="center">
  <img src="assets/logo.png" alt="Elden Trials" width="120" />

  <h1>ELDEN TRIALS</h1>

  <p><strong>Boss trial challenges for Elden Ring.</strong><br />
  Fixed builds. Real arenas. One clock.</p>

  <p>
    <a href="https://github.com/foxday/elden-trials-releases/releases/latest">
      <img src="https://img.shields.io/github/v/release/foxday/elden-trials-releases?label=latest&color=c9a86a&style=for-the-badge" alt="Latest release" />
    </a>
    <img src="https://img.shields.io/badge/platform-Windows-5b5b5b?style=for-the-badge" alt="Windows" />
    <img src="https://img.shields.io/badge/status-beta-d08a3c?style=for-the-badge" alt="Beta" />
    <img src="https://img.shields.io/badge/Elden%20Ring-1.17.1-c9a86a?style=for-the-badge" alt="Elden Ring 1.17.1" />
  </p>

  <p>
    <a href="https://eldentrials.vercel.app">Website</a> ·
    <a href="https://eldentrials.vercel.app/leaderboards">Leaderboards</a> ·
    <a href="https://github.com/foxday/elden-trials-releases/releases">Releases</a> ·
    <a href="mailto:teruelpablo@gmail.com">Contact</a>
  </p>
</div>

---

> [!WARNING]
> **Online play is not supported.** `EldenTrials.exe` already starts Elden Ring
> in **offline mode with Easy Anti-Cheat disabled**. You do not need to change
> any game, EAC or launcher settings yourself.
>
> **This is a beta.** Expect rough edges, balance changes and progress resets
> between builds.

## Your save is never touched

Elden Trials does **not** read, modify, replace or upload your Elden Ring save
under any circumstance.

- `EldenTrials.exe` launches Elden Ring through Mod Engine 3 in **offline mode**
  with the mod package and its own dedicated `elden_trials` save.
- The launcher only installs that dedicated save into the selected save folder.
  It never opens, edits or overwrites your existing characters or `ER0000.sl2`.
- Your main characters are never loaded by the mod. The game always starts with
  the dedicated `elden_trials` character.
- The mod cannot load another save or switch to one of your characters.

## About

Elden Trials is a challenge mod for **Elden Ring + Shadow of the Erdtree**.
Each trial gives you a handcrafted build, drops you into a boss arena and starts
the clock. The difficulty is mastering the build, not farming levels or running
across the map.

Every clear is submitted automatically to the online leaderboards. You can
compare your personal bests, world records and world position per trial.

The **Tarnished Edition** bundle is supported as long as it includes the
Shadow of the Erdtree expansion.

## Requirements

- **Elden Ring + Shadow of the Erdtree** (Tarnished Edition included, as long as
  it contains the expansion).
- **Regulation 1.17.1** and a game executable that matches the supported build.
- **Windows 10 or 11** (64-bit).
- A local **Elden Ring installation**.
- Enough free space for the mod package and the dedicated save.

### Steam detection

The launcher detects whether Steam is installed:

- **Steam detected:** the launcher reads your Steam library and automatically
  fills the game path and the save folder. In this mode **Steam must be running**
  when you start the mod.
- **Steam not detected:** the launcher asks for the `eldenring.exe` path and the
  folder where the dedicated save should be installed. Steam is not required in
  this mode.

In both modes the mod uses the same dedicated `elden_trials` save and never
reads or modifies your existing Elden Ring save.

Mod Engine 3 is bundled with the release. You do **not** need to install .NET,
Visual C++ runtimes or Mod Engine separately.

## Download

Download the latest `EldenTrials-<version>.zip` from
[GitHub Releases](https://github.com/foxday/elden-trials-releases/releases/latest).

Only download Elden Trials from this repository. Mirrors and reuploads are not
supported.

## Installation

1. Download the latest release ZIP.
2. Extract it to a writable folder, for example `C:\Games\EldenTrials`.
   - Do **not** extract it inside the Elden Ring installation folder.
3. Run `EldenTrials.exe`.
4. The first launch opens the setup screen:
   - it checks the game build;
   - if Steam is detected, it auto-completes the game path and save folder;
   - if Steam is not detected, it asks for `eldenring.exe` and the folder where
     the dedicated save will be installed;
   - it asks for your player name if the account is new.
5. Press **Play**. The launcher starts Elden Ring through Mod Engine 3 in
   offline mode with the mod package and the dedicated save.

If Steam was detected, keep Steam running while you play. Without Steam, the
manual paths you selected are used instead.

Always start the game through `EldenTrials.exe`. Launching Elden Ring directly
will not load the mod.

### Windows SmartScreen

The launcher is not code-signed, so Windows may show a SmartScreen warning.
Choose **More info → Run anyway**, but only if the ZIP came from this official
repository.

## First launch and account

The setup screen has two possible flows:

**Steam detected**
- The launcher reads your Steam library and fills the game path and save folder
  automatically.
- Steam must be installed and running when you press **Play**.
- If your Steam account already has an Elden Trials player, your progress is
  restored. Otherwise choose a free player name.

**Steam not detected**
- Select `eldenring.exe` manually.
- Select the folder where the dedicated save will be installed.
- Choose a player name to create the account.

In both cases the launcher never reads your existing characters; it only places
the dedicated save.

- Your account, token and settings are stored in `%APPDATA%\EldenTrials`.
- If you create a new account, **save the recovery code shown once**. It is the
  only way to recover the account on another PC.
- Leaving the name empty starts the game without a leaderboard account.

## How to play

1. Start Elden Trials with `EldenTrials.exe`.
2. Complete the setup screen and press **Play**.
3. In Elden Ring, choose **Continue** or **Load Game**.
4. Load the **`elden_trials`** character.
5. Go to the **Roundtable Hold** and sit at the grace.
6. In the grace menu, select **Elden Trials**.
7. Choose the mode (**Normal** or **No Hit**), then select a challenge.
8. Review the fixed build on the card and press **START**.
9. Defeat the boss. Your time is submitted automatically and your personal
   best, the world record and your world position are updated.

Press the website shortcut shown in the selector, or `Y` on a gamepad, to open
your player profile and leaderboards in the browser without interrupting the
run.

## Updating

From **v0.5.0** onward, the launcher checks GitHub Releases and can update
itself. The updater downloads the new ZIP, verifies its SHA-256 hash, keeps a
backup and replaces the launcher, overlay, mod package, data and dependencies
while preserving `config` and `dist`.

- Installations **older than v0.5.0** must install v0.5.0 manually once. After
  that, updates can be automatic.
- New challenge content can also be delivered through the remote catalog
  without reinstalling the mod.
- Your account lives in `%APPDATA%\EldenTrials`, not inside the mod folder.

## Troubleshooting

| Problem | What to try |
| --- | --- |
| Steam is not detected | Select `eldenring.exe` and the save folder manually in the setup screen. |
| The game does not start with Steam installed | Start Steam, keep it running and launch `EldenTrials.exe` again. |
| Windows blocks the launcher | SmartScreen → **More info** → **Run anyway**. Verify the ZIP came from this repository. |
| The game starts without the mod | Start it with `EldenTrials.exe`, not directly. |
| Unsupported game build | The mod uses fixed executable offsets. Use the supported regulation/build (1.17.1). |
| The `elden_trials` character is missing | Check that the correct save folder was selected in the setup screen. |
| Antivirus quarantines files | Restore the files and add the Elden Trials folder as an exception. |
| The overlay or selector does not appear | Close the game and check the logs below. |
| Account lost | Use the recovery code. Without it, the account cannot be restored. |

Logs:

- `dist\equipment-runtime\equipment.log`
- `dist\equipment-runtime\cards-overlay.log`

When reporting a problem, include what you were doing, what you expected, what
happened, and a screenshot if possible. You can open an issue or email
[teruelpablo@gmail.com](mailto:teruelpablo@gmail.com).

## Uninstall

1. Close Elden Ring and the launcher.
2. Delete the Elden Trials folder.
3. Optional: delete `%APPDATA%\EldenTrials` to remove the local account, token
   and settings.
4. Your Elden Ring installation and main save are not modified by the mod.

## FAQ

**Does it modify or use my main save?**  
No. Elden Trials never reads, modifies or replaces your Elden Ring save. The
launcher starts the game offline with a dedicated `elden_trials` save; your
existing characters are never loaded.

**Can I play with my main character?**  
No. The mod always launches with the dedicated `elden_trials` character and
cannot load another save.

**Can I play online?**  
No. `EldenTrials.exe` always launches the game in offline mode and handles
Easy Anti-Cheat automatically. You do not need to disable anything manually.

**Do I need the DLC?**  
Yes. Shadow of the Erdtree is required.

**Do I need Mod Engine 3?**  
It is bundled with the release. You do not need a separate installation.

**Do I need Steam?**  
It depends on your setup. If Steam is installed, the launcher auto-detects the
game and save paths, and Steam must be running when you play. If Steam is not
detected, you can point the launcher to `eldenring.exe` and the save folder
manually and play without it.

**Is my progress stored online?**  
Your times and account live online. The mod folder only contains the game
package, save and configuration.

## Links

- Website: <https://eldentrials.vercel.app>
- Leaderboards: <https://eldentrials.vercel.app/leaderboards>
- Releases: <https://github.com/foxday/elden-trials-releases/releases>
- Contact: [teruelpablo@gmail.com](mailto:teruelpablo@gmail.com)
- Nexus Mods: *coming soon*

## Credits

- **PHT** — design, development and challenge creation.
- **Mod Engine 3** by garyttierney — bundled mod loader (MIT / Apache-2.0).
- **Dear ImGui** by ocornut — overlay UI.
- **MinHook** by TsudaKageyu — API hooking.
- **Cinzel, Inter and Gelasio** — overlay fonts (SIL Open Font License 1.1).
- **Font Awesome Free** — timer icons (CC BY 4.0 / SIL OFL 1.1).

## Legal

Unofficial community project. Elden Ring and Shadow of the Erdtree are
trademarks of Bandai Namco Entertainment and FromSoftware. This project is not
affiliated with or endorsed by Bandai Namco Entertainment or FromSoftware.

---

<div align="center">
  <sub>Made by PHT · <a href="mailto:teruelpablo@gmail.com">teruelpablo@gmail.com</a></sub>
</div>
