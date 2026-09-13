<p align="center">
  <img src="textures/segment2/custom_coopdx_logo.rgba32.png" alt="SM64 Co-Op DX VR" width="720">
</p>

<p align="center">
  <a href="https://github.com/fulldivegames/sm64coopdx-VR-Physics-based"><strong>PC VR edition</strong></a>
  &nbsp;|&nbsp; <strong>Quest standalone edition</strong>
</p>

<h1 align="center">sm64coopdx-VR-Standalone (Physics-based)</h1>

<p align="center">
  Native ARM64/OpenXR VR for Meta Quest. No PC is required after installation.
</p>

> **Current public release: v0.9.21 — Physical Gestures and New Power-Ups**

> [!WARNING]
> This is an active, vibe-coded, yet fairly polished fan project. The standalone edition has been tested on **Meta Quest 3 only**. It has **not been tested on Quest 2 by me**, and neither edition has been tested across every multiplayer situation, ROM hack, or mod combination. Occasional crashes or issues might occur. If you have any performance issues on default settings in the base game, a reset usually fixes things (You should be getting a stable 120 FPS on Quest 3, on most if not all base game maps)

> [!WARNING]
> Standalone co-op, Chat, and its VR keyboard are still experimental. Text or other menu elements may occasionally appear blurry or visually incorrect; restarting the app or headset usually clears these issues. Co-op can also produce minor visual bugs. Large lobbies may reduce performance, and gameplay-changing server mods can cause visual problems, broken behavior, or crashes. Disconnecting may recover the session; otherwise, fully restart the game. Controller keyboard text chat is available.

### New in v0.9.21 — Physical Gestures and New Power-Ups

- Added Speed Running Mode (Vanilla Game), optional Vanilla Movement (Restrictive Jumps), and Disable Punch Sound for physical punches only; saved preferences and jump/jump-kick sounds are preserved.

- Added Propeller Mushroom: a 60-second power-up with an airborne burst, slow glide, crouch-controlled spinning descent, stomp rebounds, and a customizable propeller helmet.
- Added Power Star: 30 seconds of enemy-contact invincibility, 1.5x running speed and jump height, rainbow shimmer, torso sparkles, and dedicated music with a four-second expiry fade. Its bouncing pickup floats on water surfaces.
- Added physical jumping and swimming. Jump with either/both fists, sustain height by holding a fist up, and use gestures for jump chains, wall kicks and Propeller bursts. Swimming supports alternating strokes and overhead upward pulls.
- On the first 0.9.2 launch, physical jumping, swimming, punching, grabbing, climbing, swing release and motion dives are enabled for everyone. Physical crouching is unchanged. You can disable these actions again; later launches retain your choices.
- Added optional trigger-based jumping, adjustable physical crouch depth, and stronger climb-release jumps for hard swings.
- Added relative power-up spawn weights, grouped Power-Ups / Specials / Gestures, and optional 60-second timers for Big Hands and Power Star. Both Specials have half the ordinary spawn weight at equal slider settings.
- Added cosmetic power-up helmets and cap-state matching when grabbing your hat; updated the in-game tutorial for current controls and power-ups.

Fixes and refinements
- Improved PC physical jump recognition using tracked hand travel, and restored the jump-kick voice without re-enabling incidental airborne punch sounds.
- Hardened native and menu text against inherited fog, texture and alpha state; improved long-text handling and reduced redundant word-measurement work.
- Smoothed body tracking and corrected carried/thrown camera anchoring. Physical wall kicks retain full jump height while the triggering fist stays raised.
- Improved swimming, surface shell riding, crouch/head-height handling, and gesture separation to reduce accidental punches and dives.
- Corrected power-up music selection, replacement, held-cap size, and Propeller activation after small jumps, water exits and surface contacts.
- Improved PC shader compatibility, OpenGL backend selection, and updater transfer handling. Existing saves, mods, palettes and other options are retained.

PC: extract the complete ZIP, including speech and music assets. No ROM is supplied. PC speech under Wine/Proton and untested GPU/runtime combinations are not certified.

See the [v0.9.21 release](https://github.com/fulldivegames/sm64coopdx-VR-Standalone-Physics-based/releases/tag/v0.9.21) for downloads. No ROM is included.

### Multiplayer and public-lobby safety

This is an unofficial, unauthorized fan build and is not endorsed by the SM64 Co-Op DX or Nintendo teams. **Public VR Lobbies** are intended for this project's Quest standalone and PC VR builds. **Regular Public Lobbies** use the compatible Android public directory; all VR cheats and power-ups/special moves are disabled there. Play regular public lobbies at your own risk and follow the server rules. Private lobbies and direct connections remain available for invited cross-platform sessions.

VR nametags are disabled by default in v0.7.7 because their world-space placement still needs additional work. They can be enabled manually in the multiplayer HUD settings for testing.

### Voice chat

Compatible Quest standalone and PC VR clients include built-in voice chat for Public VR Lobbies and supported private/direct sessions. It also works for flat-screen players using the matching PC build. Quest always uses the headset microphone.

Open **Server Settings > Voice Chat** to enable or disable voice chat, mute your microphone, adjust microphone level, or adjust other-player volume. The **Players** menu supports individual two-way mutes and shows a speaker icon beside players who are actively speaking. The on-screen keyboard's microphone button can also dictate speech into the active text field. This project's voice traffic is not sent in Regular Public Lobbies.

This repository contains the standalone Android/Quest port of [sm64coopdx-VR (Physics-based)](https://github.com/fulldivegames/sm64coopdx-VR-Physics-based), derived from [SM64 Co-Op DX](https://github.com/coop-deluxe/sm64coopdx). It runs the game natively on the headset through OpenXR and OpenGL ES while retaining the original project's multiplayer foundation, Lua/mod support where compatible, first- and third-person cameras, tracked hands, and physical VR interactions.
There are videos on my YouTube channel: https://www.youtube.com/@fulldivegames667 that show off the mod.

## Download and install with SideQuest

The release is a single APK. Players do not need Git, Android Studio, Gradle, ADB commands, or a PC VR streaming application.

### Requirements

- Meta Quest 3 (Quest 2 untested by me, but should run fairly well. There are also performance options!)
- Developer Mode enabled for the headset
- [SideQuest](https://sidequestvr.com/setup-howto) installed on a computer
- A USB data cable or an already configured SideQuest wireless connection
- Your own legally obtained, unmodified **Super Mario 64 US `.z64` ROM**

### Install the APK

1. Open this repository's [latest release](https://github.com/fulldivegames/sm64coopdx-VR-Standalone-Physics-based/releases/latest).
2. Download `SM64-Co-Op-DX-VR-Quest-v0.8.4.apk` under **Assets**.
3. Connect the Quest to your computer and allow the USB debugging prompt inside the headset.
4. Open SideQuest and confirm that the headset indicator is connected.
5. Click **Install APK file from folder** in SideQuest, choose the downloaded APK, and wait for the install-success message.
6. In the headset, open the App Library, select **Unknown Sources**, and launch **SM64 Co-Op DX VR**.
7. On first launch, use the Android file picker to select your own unmodified US `.z64` ROM. Placing the ROM in the headset's **Downloads** folder beforehand makes it easy to find.
8. After the ROM finishes importing, the app will likely close. This is expected; simply reopen **SM64 Co-Op DX VR** from **Unknown Sources**.
9. Stand comfortably, face forward, and use **Settings > VR > Recalibrate Tracking** if the initial height or direction is wrong.

### Updating an existing installation

1. Launch **SM64 Co-Op DX VR** and wait for the title screen.
2. When a newer standalone build is available, select **Update available: vX.Y.Z - Install**.
3. If Quest opens the install-permission screen, allow installs for **SM64 Co-Op DX VR** and select the update button again.
4. Wait for the download-complete message, approve the Android installer prompt, and let the app relaunch after installation.
5. Install updates over the existing app; do not uninstall first if you want to preserve the private ROM, saves, and settings. Back up important saves before testing a new release.

> [!IMPORTANT]
> The APK contains no ROM and no Nintendo game assets. Do not upload, bundle, or redistribute a ROM with this project. The app validates the unmodified US ROM before importing it into private application storage.

## Install mods on Quest standalone

The standalone build loads compatible SM64 Co-Op DX mods from this easy-to-access folder on the Quest:

```text
/sdcard/SM64VR/mods/
```

1. Install or update to v0.8.4 and launch it once. Android opens the **Allow access to manage all files** page; enable access for **SM64 Co-Op DX VR Standalone**. This permission is used for the shared mod, DynOS, palette, and shader-cache folders.
2. Close and reopen the game once after granting access. The game creates `/sdcard/SM64VR/mods/` automatically.
3. Download a mod compatible with SM64 Co-Op DX. The official community browser is [mods.sm64coopdx.com](https://mods.sm64coopdx.com/mods/).
4. Extract the archive. Copy the **extracted mod folder**, not the `.zip`, into `SM64VR/mods` with SideQuest's file manager. The mod files must be directly inside their own folder rather than inside an extra duplicate folder.
5. Fully close and reopen **SM64 Co-Op DX VR**. From the main menu, open **Host > Mods**, select the installed mod, and start the game. Use **Refresh** if the mod was copied while the app was open.

You can also create the folder and transfer an extracted mod with ADB:

NOTE: If you have a lot of mods, your game might take longer to load or sometimes not respond when launching. Resets or waiting often works.

```powershell
adb shell mkdir -p /sdcard/SM64VR/mods
adb push "C:\path\to\ExtractedModFolder" /sdcard/SM64VR/mods/
```

The previous private `Android/data/com.fulldivegames.sm64coopdxvr/files/mods/` location remains a compatibility fallback. If the special file-access permission is declined, mods already stored there continue to load, but `/sdcard/SM64VR/mods/` is unavailable.

### Install DynOS packs

Launch the game once after installing v0.8.2. The game automatically creates:

```text
/sdcard/SM64VR/dynos/packs/
```

Extract each DynOS pack and copy its complete pack folder into `SM64VR/dynos/packs` using SideQuest's file manager. For example:

```text
/sdcard/SM64VR/dynos/packs/My Character Pack/
```

Restart the game after copying packs, then enable them from the game's DynOS menu. Copy the extracted folder rather than the downloaded archive, and avoid an extra duplicate nesting level such as `My Pack/My Pack/files`.

Custom palette files can be copied to:

```text
/sdcard/SM64VR/palettes/
```

The persistent learned shader cache is stored in `/sdcard/SM64VR/shader-cache/`. It is managed by the game; do not install mods there.

### Mod compatibility in v0.7.2

v0.7.2 includes expanded mod discovery, startup, menu, rendering, character-model, DynOS, and palette path compatibility. Character Selector was specifically tested with multiple character packs, including its in-game selection overlay. Multiple extracted DynOS packs are discovered from `dynos/packs`, and shared standalone paths now keep mods, packs, palettes, and shader-cache data accessible outside Android's restricted private-data folder.

Compatibility is not universal. Mods that depend on desktop-native binaries, desktop-only graphics APIs, unsupported keyboard windows, extreme memory use, or assumptions about the original flat camera may still fail. Character packs can also define their own selection rules rather than appearing in the built-in Mario/Luigi/Toad/Wario/Waluigi list. Install one mod at a time when diagnosing a failure and report the exact mod name/version with a crash log when possible.

Not every desktop mod is compatible with the standalone ARM64/OpenGL ES build. Mods that depend on desktop-only code, very large model or texture packs, and demanding ROM hacks may fail to load or run poorly. Install one mod at a time when troubleshooting. Only download mods you trust, and do not redistribute copyrighted game assets.

Known compatibility notes:

- Loading many mods at once can increase startup time and memory use.
- Render96 currently has known performance issues on standalone.
- Character Selector's in-game overlay was tested with multiple character packs for v0.7.2, but especially large or incompatible character packs can still cause instability.

## Tutorial: controls and how to play

### Default Quest controls

| Action | Default input |
| --- | --- |
| Move | Left thumbstick |
| Smooth turn / camera | Right thumbstick |
| Jump / cannon fire | Right Primary (A) |
| Attack / interact | Right Secondary (B) |
| Crouch | Left Trigger |
| L button | Left stick click |
| R button | Right stick click |
| Pause | Left Menu button |
| Close fist / physical grab | Hold that hand's Grip |
| Optional button punch | Right Trigger; disabled by default |

Open **Settings > VR > Controller Bindings** to exchange the movement/camera sticks, remap the listed actions, or disable individual bindings.

### First-person mode and movement

First Person Mode is the default. The headset controls the view and, by default, Mario's forward direction. The stick controls travel while Mario retains his established acceleration, momentum, skids, jumps, and landings. Camera Settings can instead use the left or right controller as the calibrated facing source.

Swimming, Wing Cap flight, shell riding, cannon aiming, and pole dismounts follow the configured look direction. Looking up or down controls vertical swimming and flight. A normal action press is still required for swimming strokes.

### Punching

Hold a Grip to close that glove, then make a deliberate punching motion. The tracked glove is the attack point; Mario's body does not need to face the target. Punch speed, travel distance, grip threshold, and collider length are adjustable under Motion Control Settings.

### Grabbing, carrying, and throwing

Close either Grip while its glove overlaps an object the original game permits Mario to carry, such as a Bob-omb, Mips, or a baby penguin. Keep holding to carry it at the hand. Release gently to drop it, or release while moving the hand to throw it. Taking damage forces the normal game drop even if the Grip remains held.

Normal, Wing, Metal, and Vanish Caps can also be collected by touching them with a tracked glove.

### Motion-controlled diving

Punch both hands forward within the configured timing window. In the air this can trigger a dive; while running fast enough on the ground it can trigger a running dive. Air and ground motion dives have separate switches.

### Physical crouching and ground pounds

Lower the headset below roughly two-thirds of the calibrated standing height to hold Mario's crouch. Crossing that threshold while airborne triggers a ground pound. This option is enabled by default under Immersion.

### Bowser

Reach either glove to Bowser's tail and hold that Grip. Swing the held hand around your body to build spin speed, then release to throw in the physical hand-swing direction. The camera stick can assist turning, and acceleration/maximum speed are adjustable.

### Physical climbing

Physical climbing is enabled by default, while Mario's standard automatic climbing is disabled by default.

- **Poles and trees:** touch one with a glove and hold Grip. Pull yourself, change anchors with the other hand, or release both hands to fall. Hold the movement stick downward while gripping to slide down. Near the top 3% of a pole/tree—or once the headset is within the top detection window—Jump performs Mario's native top-of-pole flip.
- **Moving poles:** the player, grip anchor, collision, and visible pole follow the platform together.
- **Hangable ceilings and monkey bars:** hold Grip before or while jumping into the actual underside, then alternate hands to move. The body is hidden during the physical climb to prevent clipping.
- **Ledges:** move the headset over a safe ledge and release Grip to finish onto the top. A fast release can swing off toward the configured facing direction.
- **Native ledge body:** Model Settings > Body Settings > Hide Body While on Ledges is enabled by default for ledge grabs, hangs, climb-downs, and pull-ups.
- **Climb Any Wall or Ceiling:** the disabled-by-default Cheats option permits close fresh grips on ordinary walls and overhead ceilings. Floors, boxes, cap blocks, and breakable blocks remain excluded.

### Collection gestures

- During a star/key collection screen, hold **Grip + Trigger** on either hand to show Mario's peace-sign glove.
- During a successful painting/course exit, bring either **Grip + Trigger** hand to the headset or just above it to pull off the cap. Keep holding to carry it; release to throw it. The cap can be picked up again or returned to Mario's head. The disabled-by-default **Grab Cap at Any Time** option enables this throughout play.

### Third-person mode

Third Person Mode centers the stereoscopic view on Mario and is intended for conventional gamepad play. It remains independent of first-person tracked-hand and body-camera behavior, supports the default and free cameras, and can be used to play through the normal game without motion-control gestures.

## Power-ups and special moves

### Fire Flower

Fire Flower is enabled by default under **VR > Special Moves**. Supported coin/1-Up item boxes have a 50% flower chance and supported cork boxes have a 30% chance. While powered up, close the right glove with Grip, hold Right Trigger to charge an orange fireball, then physically swing and release Trigger to throw it. The normal Attack button fires a quick shot outside first-person mode. Fire Mario's palette and music end with the power-up; **Cheats > Spawn Menu** can create a Fire Flower and **No Fire Flower Timer** keeps the power until a room transition.

### Rasengan and Rasen-Shuriken

**Rasengan / Rasen-Shuriken** is enabled by default under **Special Moves**. Hold Right Trigger with an open right hand and circle a closed, empty left glove around it until the Rasengan finishes charging. Keep holding Right Trigger to retain it, then touch a supported enemy or breakable box with the sphere. The optional **Rasengan Grip + Trigger** setting replaces the circling gesture.

With a charged Rasengan held, hold the mapped **Special** button—Y/Left Secondary by default—while keeping the hand above the headset when **Rasen-Shuriken Overhead Charge** is enabled. Once charged, physically swing and release Right Trigger to throw it. It flies until it strikes geometry or a supported enemy, then expands into a rotating area-damage sphere for 1.5 seconds and fades over 0.5 seconds. Entering the sphere causes one Bob-omb-strength hit; remaining inside for its complete lifetime causes a second. King Bob-omb and Whomps accept these moves only through their back weak spots, preserve their native multi-hit boss rules, and retain normal grab behavior. Charge-time sliders are available in **Cheats**.

### Level Select and Spawn Menu

Open **Settings > VR > Cheats** while in a game:

- **Level Select** opens a scrollable list of the castle areas, all main courses, secret stages, cap stages, Bowser stages/arenas, and the ending. Courses with missions enter through their normal Act Select path.
- **Spawn Menu** creates a Wing Cap, Vanish Cap, Metal Cap, or Fire Flower above Mario. Close the menu to let the selected pickup fall into the level.

These are cheats and can bypass normal progression. They do not alter save data unless normal gameplay inside the destination does so.

### Custom color-palette selector

Open the player palette editor and choose **Color Palette** to open the controller-friendly quick selector. It provides 44 distinct named colors, including direct red/blue values, neutrals, skin tones, metallic colors, and extended crayon-style shades. Selecting a color returns to the editor and writes its RGB/hex value into the currently selected character part; Back exits without changing it. Normal RGB sliders and hex editing remain available.

Custom presets remain saved in `/sdcard/SM64VR/palettes/`. The generated **Fireflower** preset controls the temporary Fire Flower outfit, so players can edit that preset to customize their powered-up colors; the previously selected normal palette is restored when the power ends.

## Comfort, immersion, and visual options

All options in **Settings > VR > Immersion** default to enabled:

- Smooth crouch and sinking-surface camera motion
- Full-view face-stuck blackout with readable stereo text
- Cannon aim-direction cone, firing lockout, and four directional arrows
- Head-tracked horizontal 3D positional sound
- Camera movement with Mario's ledge catch and pull-up animation
- A light 25%-opacity castle-water-blue filter only while the headset is underwater
- Side-flip camera follow
- 180-degree wall-jump camera turning
- Physical crouching and ground pounds

Painting entries use a short white comfort fade. The optional True First Person and True Diving camera effects remain experimental and can cause motion sickness.

## Settings overview

| Submenu | Main controls |
| --- | --- |
| Camera Settings | Camera mode, height/position, previous Mario body height, FOV, facing source, facing calibration, and standalone color controls |
| Controller Bindings | Motion-controller enablement, stick selection, button mappings, and optional trigger punch |
| Motion Control Settings | Punching, grabbing, climbing, dives, jump turning, hit ranges, and Bowser tuning |
| Model Settings | Body visibility/placement, feet-only, ledge and pole-flip visibility, glove scale, rotation, and position |
| Performance | Render scale from 10%-100% (80% default), optional FPS counter, 72/90/120 Hz refresh selection, fog control, flame/lava optimization, and Ultra Performance Mode |
| HUD Settings | HUD opacity and corner spread |
| Immersion | Default-on comfort, audio, camera, underwater, cannon, and physical-crouch options |
| Effects | Twirl tornado visual effect and optional normal maps |
| Cheats | Level Select, Spawn Menu, climb-any-surface, special-move charge times, flying speed, swimming speed, and running speed |
| Experimental | True First Person, True Diving, Arms Mode, and original movement options |

## Standalone-specific notes

- Quest color grading uses slightly deeper saturation and contrast than the PC build to reduce the washed-out appearance seen on Quest 3. The Brightness value itself is unchanged.
- The game keeps Super Mario 64's deterministic 30 Hz gameplay simulation while rendering and tracking at the headset cadence. Physics are not globally accelerated.
- Render Scale defaults to 80% and can be adjusted from 10% through 100%. Lower it if a demanding level or mod cannot maintain headset refresh. Menus remain full resolution.
- Refresh Rate offers 72, 90, and 120 Hz and defaults to 120 Hz on both Quest 2 and Quest 3. The selected target is not a guarantee that every level or mod can maintain that frame rate.
- **Ultra Performance Mode** reduces selected cosmetic effects and animation costs without removing enemies, signs, boxes, objectives, or other gameplay actors. Its warning accurately notes that visuals are degraded.
- Public CoopNet lobbies are shared with **Meta Quest first, and other compatible Android builds** using the same SM64 Co-Op DX network version. The standalone public directory is separate from the PC public directory.
- To play with a version-matched PC build, use **Direct Connection**. Private password rooms retain the compatible desktop namespace, but Direct Connection is the clearest supported PC/standalone route.
- Online co-op has not been comprehensively validated across every player count, mod combination, or network condition.
- Large Lua mods, model packs, ROM hacks, and texture packs may exceed standalone memory/performance budgets or rely on desktop-only behavior.

When **WiddlePets** is enabled, Server Settings adds a **Pets** button that opens the mod's own `/wpets` pet-selection menu. Pet choice, spawning, and following behavior remain controlled by WiddlePets itself.

## v0.8.4 — SteamVR and Controller Binding Fixes

- Added reliable SteamVR/OpenXR runtime handoff behavior, including ALVR compatibility through SteamVR, without forcing a particular system runtime.
- PC and Quest now use their matching GitHub release feeds, so PC VR updates resolve to the PC VR repository while Quest updates remain on the standalone repository.
- Added controller-binding capture that waits for the next input, supports remapping, and keeps the right-primary menu A action independent from the gameplay Jump binding.
- Added optional texture-matched normal maps with configurable strength and gloss controls. Normal maps are off by default; PC VR ships with 300% strength and 170% gloss.
- Stabilized PC first-person camera height/recenter calibration and thumbstick-turn lighting state while keeping Quest tracking behavior unchanged.
- Kept Sonic Shoes audio and power-up behavior synchronized across the PC VR and Quest builds.

## v0.8.3 — Quest First-Run and Updater Fix

- ROM selection now appears first on a fresh install, before microphone and storage permissions.
- Importing a valid ROM launches the game automatically instead of leaving the player at the launcher.
- Kept the selectable main-menu updater button and latest Quest APK lookup; bumped the package to v0.8.3.

## v0.8.2 — Updater and Release Notes Update

- Added the in-game standalone updater, which checks the latest standalone GitHub release, downloads the APK, installs it, and relaunches the game
- Added title-screen Release Notes pages sourced from the standalone repository
- Added clear update feedback and permission guidance during the Quest installation flow

## v0.8.0 — Sonic Shoes Update

- Added **Sonic Shoes** as a timed spawnable power-up with matching pickup gravity, Spawn Menu access, balanced box-pool integration, Green Hill Zone music, and a close-tracking sparkle trail
- Added a 0–300 Sonic speed slider with a 3× baseline at zero; the multiplier consistently covers running, acceleration, turning, slopes, dives, and dive recovery
- Added high-speed water running while Sonic Shoes are active; water behaves as a temporary surface above the threshold and safely returns Mario to swimming after slowing, bonking, or losing the power-up
- Added the compatible **WiddlePets** selection menu and its in-game location reminder without changing the mod's pet behavior
- Added reliable hammer knockback against Bully-type enemies and 1.5× knockback for special-move explosions
- Kept the performance pass conservative: reduced avoidable loading/runtime work without lowering normal visual quality or changing established gameplay behavior

## Previous Release Notes

### v0.7.9 — Voice Chat and Filters Update

- Added built-in voice chat for compatible Quest and PC VR clients, including Quest headset-mic support, microphone and player-volume controls, and a master voice-chat toggle
- Added individual two-way player muting, an active-speaker icon in the Players menu, and microphone dictation for the controller-operated keyboard
- Added the approved **Virtual Boy** and **Game Boy** full-scene filters with improved actor visibility while leaving normal rendering unchanged
- Added a conditional **Pets** shortcut to Server Settings when WiddlePets is active; it opens the mod's real pet-selection and following menu
- Hardened Rasengan and Rasen-Shuriken model lookup for ROM hacks such as B3313 without changing their charge, combat, physics, or visual behavior

### v0.7.2 — Boss Combat, Spawn Tools, and Camera Fixes

- Added **Cheats > Spawn Menu** with Wing Cap, Vanish Cap, Metal Cap, and Fire Flower buttons while retaining the complete scrollable Level Select
- Expanded Rasengan and Rasen-Shuriken interactions across giant Goombas, Pokeys, breakable boxes, Whomps, King Whomp, and King Bob-omb while preserving protected actors and native boss progression
- Added the persistent Rasen-Shuriken explosion volume: one hit on entry, a second hit only after continuous full-duration exposure, a 1.5-second hold, and a 0.5-second fade
- Tightened King Bob-omb's physical grab and special-move activation to a back-sized weak spot without changing ordinary Bob-ombs or other normal grabbables; impact visuals still wrap his complete model
- Added rear Fire Flower damage to King Bob-omb as one native boss hit and stabilized Whomp reactions so attacks cannot leave them trapped in an invalid action
- Raised and stabilized the first-person camera/body relationship, matched moving torso height to idle height, and kept the previous-height compatibility option
- Changed **Look Toward Spawned Star** to default off for new and upgraded installs and immediately clears any residual camera blend when disabled
- Raised cork-box Fire Flower odds to 30%, retained 50% supported item-box odds, and kept the smaller pickup presentation
- Added the 44-color quick palette selector with reliable controller scrolling, direct RGB/hex application, persistent custom presets, and an editable **Fireflower** power-up palette
- Kept headset/player damage contact synchronized, narrowed physical anchoring to intended actors, and slightly extended the default punch reach without limiting its slider

### v0.7.1 — Special Moves and Level Select Update

- Added the default-on **Rasengan / Rasen-Shuriken** special move with physical charging, headset-rate animation, hand contact attacks, physical throwing, collision-triggered area damage, protected-boss rules, and configurable charge controls
- Added **Cheats > Level Select**, a scrollable in-game list covering the castle, all 15 main courses, Bowser stages and arenas, secret/cap stages, and the ending; normal courses use their native Act Select entry path
- Kept the corrected first-person Mario body relationship as the default and added **Camera Settings > Use Previous Mario Body Height** for players who prefer the earlier height
- Improved tracked hand/held-effect interpolation at 72, 90, and 120 Hz while preserving the original 30 Hz gameplay simulation
- Added and refined color-palette selection, DynOS refresh, modded HUD placement, ghost button-punch presentation, Fire Flower behavior, enemy interactions, and VR camera stability

### v0.7.0 — Chat and Fireball Update

- Added a controller-friendly in-game Chat HUD with retained recent messages, an anchored on-screen keyboard, Enter-to-send behavior, and reliable B/Back navigation
- Added a **Players** HUD directly below Chat, showing connected player names, locations, and ping; press B to return
- Improved controller keyboard navigation and repeat behavior across addresses, ports, passwords, names, Chat, and other editable fields
- Added a microphone button as a preview of future speech-to-text support; microphone transcription currently does not work and is still being developed
- Added the native VR **Fire Flower** special move, including item-box and cork-box pickups, temporary Fire Mario colors and music, tracked right-hand charging, physical fireball throws, quick button shots, enemy impacts, and settings/cheats for music, spawning, and timer behavior
- Fire Flowers are a VR-build-specific feature. They are not advertised or transferred as a public CoopNet mod and are disabled for CoopNet compatibility; use matching builds through Direct Connection for supported multiplayer testing
- Expanded fireball collision coverage, including Chain Chomp and Mr. Blizzard. Mr. Blizzard explodes, disappears, and respawns after 30 seconds
- Replaced the VR Act Select 3D stars with readable overlay stars, revealing completed missions and the next available mission in sequence
- Continued high-resolution presentation fixes for the keyboard, main-menu logo, update text, Chat, and VR menu overlays

### v0.6.27 — Co-op and Keyboards Update

- Added standalone public CoopNet lobby browsing and hosting for Quest and compatible Android players
- Added an explicit **Public / Private** lobby visibility selector so an old private password cannot silently turn a public host private
- Kept version-matched PC cross-play available through Direct Connection, while public standalone rooms remain in the Android lobby directory
- Added a full controller-operated VR keyboard for SM64 Co-Op DX text fields, including addresses, ports, passwords, names, and other editable fields
- Fixed the one-time CoopNet rules screen so **Accept Rules and Continue** is visible, controller-focused, and saved immediately
- Improved high-resolution presentation for the VR keyboard, main-menu logo, and version/update text
- Preserved private lobby, direct connection, ROM, save, settings, mod, DynOS, palette, and shader-cache behavior

### v0.6.0 — Optimization and Mod Compatibility Update

- Major renderer batching and state-change reductions, including the distant Chain Chomp/BOB performance path
- General actor, flame, lava, snow/effect, menu, shader-preparation, and startup optimizations
- 72/90/120 Hz refresh-rate selector with the same 120 Hz default on Quest 2 and Quest 3
- Correct HUD opacity behavior across coins, stars, keys, timer, camera status, and the power meter while keeping the optional FPS counter readable
- Expanded shared paths for Lua mods, DynOS packs, custom palettes, and learned shader-cache data
- Character Selector and multi-character-pack compatibility work, including a readable stereoscopic selection overlay
- Safer asynchronous Quest text-entry teardown, fixing the player-count/server-menu crash when B closes an active field
- Continued first- and third-person camera, physical interaction, climbing, controller, comfort, and mod-rendering compatibility work

## Troubleshooting

- **App is missing:** open the App Library's **Unknown Sources** category.
- **ROM picker rejects the file:** use an unmodified US `.z64` ROM. Other regions and modified ROMs are not accepted.
- **App closes after importing the ROM:** this is expected on the first import. Reopen the game from **Unknown Sources** and it should load normally.
- **Wrong height or facing:** use **Settings > VR > Recalibrate Tracking** while standing neutrally and looking forward.
- **Text, menus, or the logo look blurry:** fully restart the game or headset. A reset can clear temporary standalone VR presentation problems.
- **The VR keyboard looks wrong:** the keyboard may still show minor visual bugs. Exit the field or menu and reopen it; if that does not help, restart the game.
- **Co-op develops visual or gameplay problems:** disconnecting may restore normal behavior. If not, close and reopen the game.
- **A gameplay mod breaks the server:** gameplay-changing mods can conflict with VR or multiplayer state and may require every affected player to disconnect or restart. Test without mods before reporting a base-game issue.
- **Large lobby performance:** many connected players, actors, character packs, or synchronized gameplay mods can reduce standalone performance.
- **Text chat:** open **Chat** from the pause menu and use the controller keyboard. The microphone button is visible but speech recognition currently does not work and is still being developed.
- **Poor performance:** lower Render Scale, disable expensive mods, and restart the headset after long development/testing sessions.
- **Controls feel wrong:** reset Controller Bindings and Camera Settings, then recalibrate the selected facing source.
- **Updating fails:** uninstalling removes private app data. Prefer installing the newer APK over the existing package and back up saves first.

## Building from source

Player releases should be installed through the APK above. Developers can build from `platform/android` with Android SDK/NDK 27, Java, Gradle, CMake, and Ninja configured:

```powershell
cd platform\android
.\gradlew.bat assembleDebug
```

The debug APK is produced under `platform/android/app/build/outputs/apk/debug/`. A ROM must never be added to the repository or APK.

## Credits and legal notice

- [SM64 Co-Op DX](https://github.com/coop-deluxe/sm64coopdx) and the Coop Deluxe Team
- [sm64ex-coop](https://github.com/djoslin0/sm64ex-coop) and its contributors
- The Super Mario 64 decompilation and PC-port contributors
- [Khronos OpenXR](https://www.khronos.org/openxr/) and Meta's Android/OpenXR platform components
- Lua 5.3.5, included under its MIT-style license in `platform/android/third_party/lua-5.3.5/doc/readme.html`

This is an unofficial fan project and is not affiliated with or endorsed by Nintendo, Meta, the SM64 Co-Op DX team, SideQuest, or Khronos. Super Mario and related names, characters, and assets belong to their respective owners. This repository does not grant permission to redistribute Nintendo ROMs or game assets.
