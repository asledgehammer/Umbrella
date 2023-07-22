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
3) Create new project.
4) Clone the repository into a folder.
5) `cd [your folder]`
6) `git submodule update --init --remote`
7) Have fun!

If you want to use Umbrella with **IntelliJ IDEA**, you need to use a build from before 2023 as modern **[EmmyLua](https://plugins.jetbrains.com/plugin/9768-emmylua)** doesn't currently support indexing. You can download older builds of IntelliJ [here](https://www.jetbrains.com/idea/download/other.html).

# Support

![](https://i.imgur.com/ZLnfTK4.png)

# Discord Server

<https://discord.gg/u3vWvcPX8f>

If you like what I do and helped your community a lot, feel free to buy me a coffee!
<https://ko-fi.com/jabdoesthings>

<https://www.paypal.com/paypalme/JabJabJab>
