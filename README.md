# Dvorax

Dvorak keyboard layout with international characters.

## xkb/Linux

![Screenshot of a keyboard layout](xkb/layout.png)

### Usage

1. Copy [dx](xkb/dx) into `/usr/share/X11/xkb/symbols`.
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

## Windows

![Screenshot of a keyboard layout](klc/layout.png)

### Usage
Open with Microsoft Keyboard Layout Creator, generate the installer, and install. The layout should appear as "German - Custom" or something similar.

