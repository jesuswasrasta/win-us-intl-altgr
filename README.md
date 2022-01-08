# United States (International) with AltGr dead keys

  - [Introduction](#introduction)
  - [Additions](#additions)
  - [Screenshots](#screenshots)
  - [Most common Alt-Gr combinations](#most-common-alt-gr-combinations)
  - [How to Build or Install](#how-to-build-or-install)

## Introduction
Windows includes a keyboard layout called "United States (International)", which allows typing many special characters easily.
The layout defines several keys as "dead keys", such as the apostrophe (`'`) and double quotes (`"`).
This means that to enter a single `'`, you have to press `'` followed by a space.
This can be annoying when you need to enter a lot of these characters, since each now requires two keys to be pressed.

In Linux, there is a keyboard layout named "USA International (AltGr dead keys)" that solves this problem and still allows typing special characters.
If you want to type `'`, you just press `'`.
If you want to use `'` as a dead key, you use AltGr (right alt): e.g. `AltGr+' a` will produce `á`.

This repo is a modified version of the default Windows "United States (International)" keyboard layout that mimics the behaviour found in Linux.
All five dead keys (`` ` ``, `~`, `^`, `'` and `"`) are now only dead when AltGr is pressed, otherwise they function as normal keys.
Note that the original layout already defines several AltGr combinations, e.g. `AltGr+'` becomes `´`.
If you want to type these characters in the modified layout, you should follow the old keycombination with a space: e.g. `AltGr+' <SPACE>` will produce `´`.

## Additions
- [Schwa: ə](https://it.wikipedia.org/wiki/Scev%C3%A0)
- [Grade: °](https://it.wikipedia.org/wiki/Grado_(simbolo)) (already present but not visibile in the layout editor)

## Screenshots
Default layout
![Default layout](images/us-int.jpg "standard")

AltGr layout
![Layout when Alt-gr pressed](images/us-intAltGr.jpg "alt-gr pressed layout")

Shift layout
![Layout when Shift pressed](images/us-intShft.jpg "shift pressed layout")

AltGr+Shift layout
![Layout when Alt-gr pressed](images/us-intShftAltGr.jpg "alt-gr pressed layout")

Ctrl layout
![Layout when Shift pressed](images/us-intCtrl.jpg "shift pressed layout")

## Most common Alt-Gr combinations
- (schwa) ə -> Alt-Gr + \
- é -> (Alt-Gr + ') + e  
- è -> (Alt-Gr + `) + e  
_... (and so on for the other vowels) ..._  
- (grade) ° -> Alt-Gr + v  

## How to Build or Install
You can download the latest installer from the releases tab of this repo (https://github.com/thomasfaingnaert/win-us-intl-altgr/releases).

If you prefer to build from source, you can open the .KLC source file in Microsoft Keyboard Layout Creator.
After opening the file, choose Project > Build DLL and Setup Package in the menu to create an installer.
