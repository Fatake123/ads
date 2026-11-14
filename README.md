# 7KBPS

A clean in-game performance panel for Minecraft 1.21.11 (Fabric). Press **Right Shift** (rebindable) to open it.

## What it does
- One-click presets: **Potato**, **Balanced**, **Quality**
- Live controls: render distance, simulation distance, max FPS, biome blend, clouds, particles, graphics mode, VSync, entity shadows, smooth lighting, view bobbing
- Saves to your normal `options.txt`

## What it does not do
7KBPS does not contain a rendering engine. The large FPS gains on weak PCs come from
**Sodium**, which is a required dependency. 7KBPS gives you a fast way to apply the
low-cost settings that matter. A fixed "60 to 120 FPS" result cannot be guaranteed:
it depends on the CPU, GPU, drivers and world.

## Build
Requires JDK 21.

    gradle wrapper        # once, if you have Gradle installed (or import into IntelliJ)
    ./gradlew build       # jar appears in build/libs/

If Gradle says a version in `gradle.properties` does not exist, copy the current
1.21.11 values from https://fabricmc.net/develop.

## Install
Put the jar in `.minecraft/mods/` together with Fabric API and Sodium for 1.21.11.

## Notes
Written against Yarn mappings. Method names can differ slightly between Yarn builds,
so a compile error in `KbpsScreen.java` is most likely a one-word rename.
