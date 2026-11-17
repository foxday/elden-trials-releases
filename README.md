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
> **Play offline.** Easy Anti-Cheat must be disabled. Use only the dedicated
> `elden_trials` save and never open modded saves or characters in online mode.
>
> **This is a beta.** Expect rough edges, balance changes and progress resets
> between builds. Do not use your main characters.

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
- A **Steam** account that has launched Elden Ring at least once.
- Enough free space for the mod package and the dedicated save.

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
   - it asks which Steam profile owns the dedicated save;
   - it asks for the player name shown on the leaderboard.
5. Press **Play**. The launcher starts Elden Ring through Mod Engine 3 in
   offline mode with the mod package and the dedicated save.

Always start the game through `EldenTrials.exe`. Launching Elden Ring directly
from Steam will not load the mod.

### Windows SmartScreen

The launcher is not code-signed, so Windows may show a SmartScreen warning.
Choose **More info → Run anyway**, but only if the ZIP came from this official
repository.

## First launch and account

The setup screen detects your Steam account from the local Elden Ring save
folders. If that Steam account already has a player, your progress is restored
automatically. If not, choose a free name and the account is created.

- Your account, token and settings are stored in `%APPDATA%\EldenTrials`.
- If you create a new account, **save the recovery code shown once**. It is the
  only way to recover the account on another PC.
- Leaving the name empty starts the game without a leaderboard account.

## How to play

1. Start Elden Trials with `EldenTrials.exe`.
2. Complete the setup screen and press **Play**.
3. Load the **`elden_trials`** character at Roundtable Hold.
4. Open the challenge selector.
5. Choose a trial, review the fixed build and press **START**.
6. Defeat the boss. Your time is submitted automatically and your personal
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
| Windows blocks the launcher | SmartScreen → **More info** → **Run anyway**. Verify the ZIP came from this repository. |
| The game starts without the mod | Start it with `EldenTrials.exe`, not from Steam. |
| Unsupported game build | The mod uses fixed executable offsets. Use the supported regulation/build (1.17.1). |
| The `elden_trials` character is missing | Check that the correct Steam profile was selected in the setup screen. |
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

**Does it modify my main save?**  
No. Elden Trials uses a dedicated `elden_trials` save. Your main characters are
not touched.

**Can I play online?**  
No. Play offline with Easy Anti-Cheat disabled. Using modded saves online can
result in a ban.

**Do I need the DLC?**  
Yes. Shadow of the Erdtree is required.

**Do I need Mod Engine 3?**  
It is bundled with the release. You do not need a separate installation.

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
