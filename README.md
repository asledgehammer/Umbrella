# Umbrella
![](https://i.imgur.com/wMKl10y.png)

Umbrella is a collection of LuaCATS typings for Project Zomboid's API. This includes:
- **[Candle](https://github.com/asledgehammer/Candle)**: The exposed Java API typings.
- **[PZLuaStubs](https://github.com/omarkmu/PZLuaStubs)**: The Lua API typings.
- **[PZEventStubs](https://github.com/demiurgeQuantified/PZEventStubs)**: The Events API typings.

## Advantages
- Types are exposed to IntelliSense through LuaCATS, showing what goes where and what's returned.
- No time spent decompiling the game and running tools to get typings. (They are provided already)
- Built using **[PZ-Rosetta](https://github.com/asledgehammer/PZ-Rosetta)**, using **[Project Zomboid's JavaDocs](https://projectzomboid.com/modding/)** to make the typings friendlier. (Parameter names, Documentation notes, etc.)

## Caveats
- Different Lua environments can behave differently. (vscode plugin, IntelliJ IDEA, etc.) This could cause issues.

# Setup

## VSCode (Recommended)

VSCode is recommended as it is the best supported Lua IDE, and its addon manager will automatically update Umbrella.

1) Install [VSCode](https://code.visualstudio.com/).
2) Open and use the extension manager to install the [Lua](https://marketplace.visualstudio.com/items?itemName=sumneko.lua) extension.
3) Install [Git](https://git-scm.com/downloads). You may need to restart your computer after installation.
4) Open your project or folder.
5) Press **Ctrl-Shift-P** and search for ``Lua: Open Addon Manager`` in the context menu that opens.
6) Search for Umbrella, and click enable. You will need to enable it for any future projects as well.
   a) For Unstable versions of Project Zomboid, use Umbrella (Unstable).

## IntelliJ IDEA

1) Install the [SumnekoLUA](https://plugins.jetbrains.com/plugin/22315-sumnekolua) plugin.
2) Download Umbrella from [Releases](https://github.com/asledgehammer/Umbrella/releases/latest) (or clone it).
3) Open/create your project.
4) Create a file named ``.luarc.json`` at the root directory of your project with the contents:
```
{
  "$schema": "https://raw.githubusercontent.com/LuaLS/vscode-lua/master/setting/schema.json",
  "workspace.library": ["path/to/umbrella"],
  "runtime.version": "Lua 5.1",
  "runtime.path": [
    "shared/?.lua",
    "client/?.lua",
    "server/?.lua"
  ],
  "completion.requireSeparator": "/",
  "workspace.preloadFileSize": 800,
  "runtime.builtin": {
    "debug": "disable",
    "io": "disable",
    "package": "disable"
  }
}
```
5) Change the ``"workspace.library": ["path/to/umbrella"]`` line to the absolute path to where you downloaded Umbrella.
6) You may need to restart your IDE to apply the changes.

## Manual Installation (Any)

1) Create new project.
2) Download the correct version of Umbrella (PZ versions used) from Releases page, or clone it.
3) Copy the downloaded folder into your project somewhere, or link it as a dependency if your IDE supports it.

## Installing Umbrella Globally

If you want to install Umbrella globally, Add a path to Umbrella via this extension setting:
![global_setup.png](./assets/media/global_setup.png)

# Support

![](https://i.imgur.com/ZLnfTK4.png)

# Discord Server

<https://discord.gg/u3vWvcPX8f>

If you like what I do and helped your community a lot, feel free to buy me a coffee!
<https://ko-fi.com/jabdoesthings>

<https://www.paypal.com/paypalme/JabJabJab>
