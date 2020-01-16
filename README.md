# C++ Chroma MOD Sample

This is a C++ console application which shows how to create a Chroma RGB lighting enabled application that is moddable.

![image_1](images/image_1.png)

The sample application has default `BASE` animations that mods can override.

```
Animations
└───Base
    ├───Fighter
    ├───Paladin
    └───Thief
```

Mods are controlled using a directory naming convention described in the [setup](#setup) section.

## Setup

Mod folders with custom Chroma animations can be placed within the application folder.

```
%USERPROFILE%\AppData\Local\Razer\CSDK_ChromaModSample
```

![image_2](images/image_2.png)

Two sample mods can be found in the `Animation` folder.

* [Mod1.zip](Animations/Mod1.zip)
* [Mod2.zip](Animations/Mod2.zip)

Both mods can be unpacked within the application folder. Mods are detected when the application starts.

```
%USERPROFILE%\AppData\Local\Razer\CSDK_ChromaModSample
├───Mod1
│   ├───Fighter
│   ├───Paladin
│   └───Thief
└───Mod2
    ├───Fighter
    ├───Paladin
    └───Thief
```

Mods use the directory template of `MOD NAME` | `CLASS NAME` | `CHROMA ANIMATION`.

Each mod has a sample class for `FIGHTER` | `PALADIN` | `THIEF`.

Each class has sample animations for `ATTACK` | `BLOCK` | `DAMAGE`.

Each animation has a device set for `CHROMALINK` | `HEADSET` | `KEYBOARD` | `KEYPAD` | `MOUSE` | `MOUSEPAD`.