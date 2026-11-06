# First Born — Forge 1.20.1

A small keepsake mod for the First Born modpack.

## What it does
- Adds one item: **First Born** (`firstborn:first_born`).
- The item cannot be crafted; this project intentionally adds no recipe.
- Right-click opens a custom parchment letter screen.
- The screen closes with the button or Escape.
- The exact supplied letter artwork is displayed as the GUI texture at `assets/firstborn/textures/gui/one_last_letter.png`.

## Give the item for testing
With cheats enabled:
```mcfunction
/give @s firstborn:first_born
```

## Give it as the final FTB Quests reward
1. Install this mod and FTB Quests on the same Forge 1.20.1 instance.
2. Open the quest book in edit mode.
3. Open the final quest in your final chapter.
4. In Rewards, press `+` and choose **Item**.
5. Search for `First Born` and add one.
6. Save the quest changes.

FTB Quests handles the reward. This mod does not need to detect quest completion itself.

## Build
Use Java 17 and Gradle. This is a ForgeGradle project; run:
```bash
gradle genIntellijRuns
gradle build
```
The built jar will be in `build/libs/`.

If you are starting from the official Forge MDK instead, copy this project's `src` folder and Gradle mod configuration into that MDK project.

## Notes
This is a source project, not a precompiled/tested JAR. Build it with the Forge 1.20.1 toolchain before putting it into your modpack.
