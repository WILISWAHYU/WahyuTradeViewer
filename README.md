# Wahyu Trade Viewer (Fabric client mod)

Target: Minecraft Java 1.21.11, Fabric, Java 21.

## What this first build does
- Client-side trade list overlay while a villager trading screen is open.
- Shows the offers currently present in the trade data the server sent to your client.
- Item display names are used, so server-sent custom item names/custom enchant names can appear.
- Press **O** to toggle the panel.

## Important limitation
This is a client-only viewer, not a server-data extractor. It cannot reveal trade offers that the server has not generated or sent to the client. Vanilla villagers may only send their currently generated offers; server plugins that keep future/custom offers hidden cannot be predicted by this mod. Custom enchantment text appears only if it is present in the item's display data sent by the server.

## Build
Open this folder in IntelliJ IDEA with JDK 21 and allow Gradle to sync, then run:

- Windows: `gradlew.bat build`
- Linux/Termux: `./gradlew build`

The compiled mod jar will be in `build/libs/`. This archive contains source project files; it is not a precompiled jar. Gradle wrapper files are not included.
