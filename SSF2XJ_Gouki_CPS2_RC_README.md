# Super Street Fighter II X — Gouki Integration

## CP21 RC • Player and enthusiast guide

This fan-made modification expands the Japanese CPS2 version of **Super Street
Fighter II X: Grand Master Challenge**, known internationally as **Super Street
Fighter II Turbo**. It makes **Gouki, Shin Gouki and Ten Gouki** selectable through
Ryu and brings their added abilities, presentation and ending into the arcade
game.

The project uses the CPS2 game engine. **Super Street Fighter II X for Matching
Service on Dreamcast** supplied reference material, artwork and animation
information. The additions were integrated into the arcade game so that play
still uses familiar six-button Street Fighter controls.

**Release status:** RC5 is an emulator-tested release candidate. Physical CPS2
hardware operation has not been verified.

## Choosing Gouki and his variants

On character select, highlight **Ryu** and press **START** to cycle:

**Ryu → Gouki → Shin Gouki → Ten Gouki → Ryu**

Confirm your choice with the usual character-select button. Both player sides
support the cycle. Moving to another character clears the Gouki selection and
restores that character's normal name and portrait.

| Character | What to expect |
| --- | --- |
| **Gouki / Akuma** | The standard arcade-based playable form, with a single air fireball and normal teleport recovery. |
| **Shin Gouki / Shin Akuma** | A boss-based form with stronger boss attack behavior, 25% faster walking, quicker teleport recovery and two air fireballs in succession. Includes Messatsu Gou Hadou. |
| **Ten Gouki / Tien Gouki** | Shares the enhanced boss-based movement and double air fireballs. Includes Messatsu Gou Hadou and adds the Raging Demon. Teleports also build meter. |

These are three versions of Gouki, sharing his original character artwork and
core move family. They are reached through Ryu's slot; Ryu remains selectable.

## Moves, super meter and finishers

All three playable forms display the **original CPS2 super bar**. Normal attacks
and special moves build meter using the full arcade-style awards. Ten Gouki also
gains meter through teleporting.

The added supers have the following assignments. Standard Gouki does not receive
these two added super commands.

| Added super | Available to | Command |
| --- | --- | --- |
| **Messatsu Gou Hadou** | Shin Gouki and Ten Gouki | Two quarter-circles forward, then any Punch. Two half-circles back plus Punch is also supported. |
| **Shun Goku Satsu / Raging Demon** | Ten Gouki | Light Punch, Light Punch, Forward, Light Kick, Heavy Punch, entered quickly. |

Both require a **full meter** and a grounded character. Forward and back are
relative to the direction your fighter is facing.

Messatsu Gou Hadou uses the arcade game's super startup and a five-hit super
fireball. The Raging Demon includes the forward approach, capture, screen
blackout, fifteen-hit sequence and release. Its miss and non-KO recovery paths
are also handled.

A super that ends the round triggers the **full arcade super-KO background
effect**. Regular fireballs, dragon punches, hurricane kicks, teleports and air
fireballs remain part of the familiar Gouki move family. Standard Gouki keeps
one air projectile; Shin and Ten use the boss-style second projectile.

## Names and presentation throughout the game

The three variants have names on **character select, the VS screen and the
battle HUD**. Selection and VS names use matching retail character-name artwork;
battle names use the arcade HUD's own font style. Their placement supports both
player sides, including the longer Shin Gouki and Ten Gouki labels.

Ryu keeps his original selection name, with the extra added label removed.
Moving around the roster clears the added name display correctly.

Player-controlled Gouki winners now use the arcade result-screen dialogue
presentation. The variants share the added English line:

> I AM THE MASTER OF THE FIST!

This is a line supplied for the modification. It is not presented as a set of
three different quotes taken from the Dreamcast game. Normal opponents retain
their own result dialogue.

**Portrait note:** Gouki's portrait areas retain the dark/blank treatment of the
base build. This release adds the finished nameplates without introducing new
portrait artwork.

## The complete Gouki ending

Completing the game with any of the three variants routes into **Gouki's full
ending**, including its portrait and animation sequence, the credits and the
return to the title flow. All three share that ending.

The Dreamcast ending was studied alongside the arcade assets. Its real artwork
already had matching CPS2 versions, allowing the existing arcade artwork and
scene machinery to be used at their original size. The added work connects a
playable Gouki victory to the full sequence and handles the transition out of
the match and onward to the credits.

## Three selectable title presentations

Open the game's **Service/Test menu**, enter **System Configuration**, and find
**TITLE**. Cycle to your preferred presentation, then exit the menu normally to
save it.

| TITLE choice | Presentation |
| --- | --- |
| **Dreamcast** | Japanese X title treatment with the original gold **for Matching Service** emblem, its blue drop shadow and connected horizontal line. |
| **Japan** | Japanese X logo and **Grand Master Challenge** subtitle. |
| **USA** | Turbo logo and **The Ultimate Championship** subtitle. |

The selection survives a normal restart. Japan is the default when no valid
saved choice is present. These settings change the title presentation; they do
not change the roster or switch the game's regional rules. The Matching Service
badge is artwork; Dreamcast online-service functionality is not included.

RC5 preserves the approved emblem artwork and corrects the subtitle's spacing
against its blue shadow and line. The title choices also retain complete
subtitle lettering.

## Intro and warning-screen improvements

The intro received repairs for blocky scene handoffs, stray sprite fragments
and graphics left behind during transitions. Input handling was checked across
the intro to address the lower-left zeros and other button-triggered debris.

The warning screen uses the requested fan-project wording, including **SSF2X**,
with the existing font style and color scheme. Its body text uses single-spaced
lines.

## Where the additions came from

| Material or feature | Origin | How it is used in this CPS2 build |
| --- | --- | --- |
| Main game, stages and fighting systems | Japanese arcade SSF2XJ | Remain the foundation for play and the new character behavior. |
| Shin and Ten abilities | Existing arcade boss behavior, with Dreamcast material used as reference | Integrated into player-controlled variants, including faster movement, quicker teleport recovery and double air fireballs. |
| Messatsu Gou Hadou | Added variant behavior using native arcade effects and projectile handling | Available to Shin and Ten with a full meter. |
| Raging Demon | Dreamcast command, sequence and animation information, combined with matching arcade poses | Recreated inside the CPS2 fighting engine for Ten Gouki. |
| Character names | Retail name and font artwork examined on the Dreamcast disc, with matching CPS2 pixels | Used to compose consistent Gouki variant labels for select, VS and HUD displays. |
| Gouki ending | Dreamcast ending reference and matching original CPS2 artwork | Connected to the playable variants' arcade ending and credits flow. |
| Matching Service emblem | Original Dreamcast disc artwork and palette | Added to the Dreamcast TITLE option, with its blue shadow and connected line. |
| Super meters and super-KO effects | Original CPS2 assets | Enabled and connected to the added playable forms and supers. |
| Attack, super and KO sound cues | Existing CPS2/QSound recordings, checked against Dreamcast references | Connected to the required added actions and the correct player side. |

Artwork remains at its native CPS2 pixel size. Release and archived asset
compression is lossless. In-game sound retains the original arcade recordings,
with the added actions connected to the appropriate cues.

The build also retains the project's existing USA boot/play-region setup and
Japanese difficulty behavior. Selecting a different title logo leaves those
settings unchanged.

## Getting started in an emulator

The verified emulator is **MAME 0.264**. Use the complete patched ROM set under
the **ssf2xj** game entry, together with the emulator's usual CPS2/QSound support
files. For the intended arcade proportions, use a **4:3** display setting.

If using the ready-to-play RC5 download, make a copy named **ssf2xj.zip** in your
emulator's ROM folder. Keep your untouched original separately. Start the new
build from a normal boot.

Modified ROMs can produce expected stock-checksum warnings. Missing-file or
loading failures still need to be resolved. Compatibility with other emulators
and frontends has not been established by the MAME checks.

## Patching your original ROM set

The separate **SSF2XJ_Gouki_CP21_RC5_IPS.zip** package upgrades the complete,
unmodified Japanese SSF2XJ ROM set directly to RC5. No earlier patch is required.

1. Extract the IPS package.
2. On Windows, with Python 3 installed, drag your original **ssf2xj.zip** onto
   **Apply_RC5.bat**.
3. The helper checks the source and writes **Gouki_RC5/ssf2xj.zip** beside it,
   preserving your original.

The package also includes a direct ZIP IPS and seven individual ROM-file IPS
patches for people who prefer their usual patcher. **PATCHING.md** explains
which file each patch applies to, the other-platform helper command and source
verification. The direct ZIP patch requires the exact original archive; the
helper also accepts repacked archives containing the same complete stock ROMs.

Both patch methods were verified to reproduce the released RC5 build byte for
byte.

## Playing on CPS2 hardware

This is a native CPS2 ROM modification, but **physical-board operation has not
been tested**. Emulator validation is not hardware certification.

Both the game program and some graphics data change. A hardware installation
must carry the complete patched data and the appropriate game/key setup for
the board or loader being used. Board compatibility, ROM preparation and
installation are outside the verified scope of this release; the IPS download
is not a board-installation kit.

## Release files and verification

| File | Purpose |
| --- | --- |
| **SSF2XJ_Gouki_CP21_RC5.zip** | Complete patched game ROM set. |
| **SSF2XJ_Gouki_CP21_RC5_IPS.zip** | Upgrade patches, application helper and player/patching guides. |
| **SSF2XJ_Gouki_Integration_Checkpoint21_RC5.zip** | Development/recovery material; unnecessary for playing. |

Focused emulator checks cover character selection on both sides, the move
families, meter gain, added supers, super-KO effects, names and result text,
ending transitions, intro inputs and saved title choices. RC5's final layout
was compared with the supplied Dreamcast reference, and its title fades were
checked after the spacing correction.

This remains a release candidate. Full unassisted campaigns and every possible
join, continue and reselect combination have not been exhaustively verified.

## Credits

Original game, characters, artwork and audio: **Capcom**. Dreamcast reference:
**Super Street Fighter II X for Matching Service**. This is an unofficial fan
modification and is not an official Capcom release.
