# Dvorax

Dvorak keyboard layout with dead keys for international characters, plus a few other tweaks. Provided with as little difference as possible across three configurations:
- Nyquist 60% keyboard under Linux or Windows, programmed with QMK, using the OS's US-International layout with dead keys.
- Standard keyboard under Linux, using XKB.
- Standard keyboard under Windows, using Keyboard Layout Creator.

## Nyquist

![Layout](https://github.com/xdlg/Dvorax/blob/master/nyquist/layout.png)

### Usage
Program the Nyquist with QMK and use the keyboard with the OS's US-International layout with dead key support.

### Notes
- "Fun" is the function layer (function keys, navigation, and volume/brightness control).
- "Sym" is the symbol layer, similar to AltGr in the other layouts.
- The key "AltTab" enables Alt-Tabbing with just one keypress.
- The key "AltGr" is provided be able to use international characters via the OS's software layout.


## Linux

![Layout](https://github.com/xdlg/Dvorax/blob/master/linux/layout.png)

### Usage

I use Linux Mint so installation steps may vary on other distributions. I chose xkb rather than xmodmap because it creates a layout that is completely integrated into the OS preferences, just like any other language layout.

 1. Copy [dx](https://github.com/xdlg/Dvorax/blob/master/xkb/dx) into `/usr/share/X11/xkb/symbols`.
 2. Add `dx Dvorax` to the layout list in `/usr/share/X11/xkb/rules/evdev.lst`.
 3. Add the following layout to `/usr/share/X11/xkb/rules/evdev.xml`:
```
<layout>
  <configItem>
    <name>dx</name>
    <shortDescription>dx</shortDescription>
    <description>Dvorax</description>
    <languageList>
      <iso639Id>ger</iso639Id>
    </languageList>
  </configItem>
</layout>
```
4. Log out and log back in. The layout should be available in the system preferences like any other language.

### Notes
- CapsLock is remapped to AltGr in order to use the navigation keys on the home row, emulating the Nyquist's "Fun" layer.
- Because of the navigation key, the symbol ß is pushed to Shit+AltGr+S (instead of just AltGr+S like on the other layouts.)


## Windows

![Layout](https://github.com/xdlg/Dvorax/blob/master/windows/layout.png)

### Usage
Open with Microsoft Keyboard Layout Creator, generate the installer, and install. The layout should appear as "German - Custom" or something similar.

### Notes
- Home row navigation keys aren't provided because KLC only supports them on the base layer.

