# Umbrella
![](https://i.imgur.com/wMKl10y.png)

Umbrella is a collection of EmmyLua typings for Project Zomboid's API. This includes:
- **[Candle](https://github.com/asledgehammer/Candle)**: The exposed Java API typings.
- **[PZLuaStubs](https://github.com/omarkmu/PZLuaStubs)**: The Lua API typings.
- **[PZEventStubs](https://github.com/demiurgeQuantified/PZEventStubs)**: The Events API typings.

## Advantages
- Types are exposed to IntelliSense through EmmyLua, showing what goes where and what's returned.
- No time spent decompiling the game and running tools to get typings. (They are provided already)
- Built using **[PZ-Rosetta](https://github.com/asledgehammer/PZ-Rosetta)**, using **[Project Zomboid's JavaDocs](https://projectzomboid.com/modding/)** to make the typings friendlier. (Parameter names, Documentation notes, etc.)

## Caveats
- Each EmmyLua environment behaves differences. (vscode plugin, IntelliJ IDEA, etc.) This could cause issues.
- Forks of EmmyLua behave differently. This can cause issues depending on use.

## Setup

1) **[Vscode](https://code.visualstudio.com/)** installed.
2) **[Lua Language Server extension](https://marketplace.visualstudio.com/items?itemName=sumneko.lua)** installed.

## Addon Manager (VSCode only)

1) Create new project.
2) Press **Ctrl-Shift-P** and search for ``Lua: Open Addon Manager`` in the context menu that opens.
3) Search for Umbrella, and click enable.

## Manual Installation

1) Create new project.
2) Download the correct version of Umbrella (PZ versions used) from Releases page.
3) Copy the downloaded folder into your project somewhere.

## Install from Repository

1) Create new project.
2) Clone the repository into a sub-folder.
3) `cd [your folder]`
4) `git submodule update --init --remote`

## Installing Umbrella Globally

If you want to install Umbrella globally, Add a path to Umbrella via this extension setting:
![global_setup.png](./assets/media/global_setup.png)

If you want to use Umbrella with **IntelliJ IDEA**, you need to use a build from before 2023 as modern **[EmmyLua](https://plugins.jetbrains.com/plugin/9768-emmylua)** doesn't currently support indexing. You can download older builds of IntelliJ [here](https://www.jetbrains.com/idea/download/other.html).

# Support

![](https://i.imgur.com/ZLnfTK4.png)

# Discord Server

<https://discord.gg/u3vWvcPX8f>

If you like what I do and helped your community a lot, feel free to buy me a coffee!
<https://ko-fi.com/jabdoesthings>

<https://www.paypal.com/paypalme/JabJabJab>
