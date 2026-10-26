# Mario + Rabbids: Community Versus Sets

A community-made mod for **Mario + Rabbids Kingdom Battle** that lets us create, share, and play custom versus sets!

You don't need any programming knowledge to contribute. If you have ideas for new sets or want to improve existing ones, you're welcome to help!


## How to make custom Versus sets

You can help by creating new versus sets, improving existing ones, or even by simply sharing your ideas on the [Mario+Rabbids Discord Server](https://discord.gg/TG4vxzkBG).

Here is how you can create your own sets:

### 1. Make your own copy of the repository

On this GitHub page, click **Fork**.

A *Fork* is your own copy of the project on GitHub. It lets you make changes without affecting the original project.

You can then download the files you want to change from there, instead of using your own extraction. This is to ensure that your changes are compatible with the rest of the mod. You can now modify them with any text editor.

### 2. Follow the contribution guide

Read the [Community Versus Sets Wiki](https://github.com/gggga00/Mario-Rabbids-Community-Versus-Sets/wiki) for instructions on how to add/modify versus sets.

The wiki also mentiones some guidelines and practices to follow when contributing.


### 3. Submit your changes

When you're happy with your changes, submit a **pull request**: [Submitting a pull request](https://docs.github.com/en/pull-requests/how-tos/create-pull-requests/creating-a-pull-request)

A pull request is a way to propose your changes to the original project. It lets us review your work before we include it in the mod.

That's it!

----------
You can reuse your fork for future contributions by syncing it to get the latest changes: [Syncing a fork](https://docs.github.com/en/pull-requests/how-tos/work-with-forks/syncing-a-fork)

Sometimes, syncing can result in merge conflicts if both repositories have changes to the same parts of a file. If this happens and you just want to get the latest version, you don't need to keep changes from your fork and can just choose the version from this repository instead.


## How to install the mod

**Before you start:** You will need your own copy of Mario + Rabbids Kingdom Battle, the game's extracted files, and either a modded Switch or an emulator.

### 1. Download the moria folder

You can download the entire repository including the `moria` folder, by clicking on **Code** and then **Download ZIP**.

### 2. Prepare the files for reimporting

Create a folder named `import` and place the downloaded `moria` folder inside it. Your folder structure should look like this:

```text
import/
└── moria/
```

### 3. Reimport the files

Use the [Mario + Rabbids ROMFS Repacker](https://github.com/gggga00/Mario-Rabbids-Reimportation-Tool)
to reimport the folder into the game's file structure.

You will need:
- Your own extracted `sdf.toc` file.
- The original `sdfdata` files `A-0016` and `A-0018`.

Follow the repacker's instructions to generate the modified files.

### 4. Install the modified files

Place the modified files in your game's mod folder. 
**It must be within the same folders in the same order as the original.**

Your folder structure should look like this:
```text
romfs/
└── moria/
    └── sdf/
        └── nx/
            └── data/
                ├── sdf.toc
                ├── A-0016
                └── A-0018
```

You will need to create any missing folders yourself.

**If you're using an emulator:**

1. Right-click Mario + Rabbids Kingdom Battle in your emulator.
2. Select **Open Mod Location**.
3. Place the `romfs` folder containing the modified files in the mod location.

**If you're using a modded Nintendo Switch:**

Place the `romfs` folder inside:

```text
atmosphere/contents/010067300059A000/
```

The resulting structure should be:

```text
atmosphere/contents/010067300059A000/
└── romfs/
    └── moria/
        └── sdf/
            └── nx/
                └── data/
```


### 5. Unlock the custom sets

Replace your `RKB1_PVP_PVP.SAVE` with the version provided in this repository to unlock the custom sets.

---


## Questions or ideas?

If you're unsure how to contribute, need help with GitHub, or have an idea for a new versus set, don't be afraid to ask over on discord!
