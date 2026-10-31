    # Curse Book — Fabric 1.21.1

Fabric 1.21.1 mod that adds a multiplayer curse book.

## Features

- Craft the book with 4 gold ingots, 4 paper, and 1 book.
- Right-click while holding the book to open the curse picker.
- Choose a curse, then choose another online player.
- Available curses: Weakness, Darkness, Mining Fatigue, Hunger, and Slowness.
- Curses last for a limited time and can be removed with `/cursebook cleanse <player>`.

The current implementation allows any player to use the book, as requested.

## Build without installing Java or Gradle

You can build this on GitHub's servers. You do not need Java or Gradle installed on your PC.

1. On GitHub, click **New repository** and name it `cursebook-mod`.
2. Set it to **Private** if you prefer, then click **Create repository**.
3. Click **Add file** → **Upload files**.
4. Open this folder on your PC and upload everything inside it:
   `C:\Users\seanc\Downloads\CurseBook-Fabric-1.21.1`
5. Confirm that the upload includes `.github/workflows/build.yml`.
6. Click **Commit changes**.
7. Open the repository's **Actions** tab.
8. Select **Build Curse Book mod**, then click **Run workflow**.
9. Wait for the green check, open the completed run, and download `cursebook-fabric-1.21.1` under **Artifacts**.
10. Extract that downloaded ZIP. The `.jar` inside is the mod.

The workflow installs Java 21 and Gradle temporarily on GitHub's build server. Nothing is installed on your computer.

Minecraft still needs Fabric Loader and Fabric API installed to run the mod. Java is already included with the normal Minecraft launcher.

## In-game usage

1. Craft or give yourself the item with `/give @s cursebook:curse_book`.
2. Hold it in your main hand and right-click.
3. Pick a curse and a player.
4. To cleanse a player, run `/cursebook cleanse <player>`.
