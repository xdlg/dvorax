# Dvorax

Dvorak keyboard layout with dead keys for international characters, plus a few other tweaks. Provided with as little difference as possible across three configurations:
- Nyquist 60% keyboard under Linux or Windows, programmed with QMK, using the OS's US-International layout with dead keys.
- Standard keyboard under Linux, using XKB.
- Standard keyboard under Windows, using Keyboard Layout Creator.

## Nyquist

![Layout](https://github.com/xdlg/Dvorax/blob/master/nyquist/layout.png)

[Keyboard Layout Editor](https://www.keyboard-layout-editor.com/##@@=Esc&_c=%23cf1d67&fa@:0&:0&:0&:0&:0&:0&:0&:1%3B%3B&=!%0A1%0A%0A%0A%0A%0A%0AF1&_c=%23f37201%3B&=%2F@%0A2%0A%0A%0A%0A%0A%0AF2&_c=%238eb734%3B&=%23%0A3%0A%0A%0A%0A%0A%0AF3&_c=%2300548c%3B&=$%0A4%0A%0A%0A%0A%0A%0AF4&=%25%0A5%0A%0A%0A%0A%0A%0AF5&_x:1&c=%2300afef%3B&=%5E%0A6%0A%0A%0A%0A%0A%0AF6&=%2F&%0A7%0A%0A%0A%0A%0A%0AF7&_c=%238eb734%3B&=*%0A8%0A%0A%0A%0A%0A%0AF8&_c=%23f37201%3B&=(%0A9%0A%0A%0A%0A%0A%0AF9&_c=%23cf1d67%3B&=)%0A0%0A%0A%0A%0A%0A%0AF10&_c=%23cccccc%3B&=BkSp%0A%0A%0A%0A%0A%0A%0ADel%3B&@=Tab&_c=%23cf1d67%3B&=%22%0A'%0A%0A%0A%0A%0A%0AF11&_c=%23f37201%3B&=%3C%0A,%0A%0A%0A%0A%0A%0AF12%0A%0A%0A~&_c=%238eb734%3B&=%3E%0A.%0A%0A%0A%0A%0A%0AF13%0A%0A%0A%60&_c=%2300548c%3B&=P%0A%0A%0A%0A%0A%0A%0AF14&=Y%0A%0A%0A%0A%0A%0A%0AF15&_x:1&c=%2300afef%3B&=F&=G%0A%0A%0A%0A%0A%0A%0APgUp&_c=%238eb734%3B&=C%0A%0A%0A%0A%0A%0A%0A%2F&uarr%2F%3B&_c=%23f37201%3B&=R%0A%0A%0A%0A%0A%0A%0APgDn&_c=%23cf1d67%3B&=L&=%3F%0A%2F%2F%0A%0A%0A%0A%0A%0A%0A%7C%0A%0A%5C%3B&@_c=%23cccccc%3B&=Fun&_c=%23cf1d67%3B&=A%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%5B&_c=%23f37201%3B&=O%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%5D&_c=%238eb734%3B&=E%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%7B&_c=%2300548c%3B&=U%0A%0A%0A%0A%0A%0A%0APrtScr%0A%0A%0A%7D&=I&_x:1&c=%2300afef%3B&=D%0A%0A%0A%0A%0A%0A%0AHome&=H%0A%0A%0A%0A%0A%0A%0A%2F&larr%2F%3B&_c=%238eb734%3B&=T%0A%0A%0A%0A%0A%0A%0A%2F&darr%2F%3B&_c=%23f37201%3B&=N%0A%0A%0A%0A%0A%0A%0A%2F&rarr%2F%3B&_c=%23cf1d67%3B&=S%0A%0A%0A%0A%0A%0A%0AEnd&=%2F_%0A-%0A%0A%0A%0A%0A%0A%0A+%0A%0A%2F=%3B&@_c=%23cccccc%3B&=Shift&_c=%23cf1d67%3B&=%2F:%0A%2F%3B&_c=%23f37201%3B&=Q&_c=%238eb734%3B&=J&_c=%2300548c%3B&=K&=X&_x:1&c=%2300afef%3B&=B%0A%0A%0A%0A%0A%0A%0AMute&=M%0A%0A%0A%0A%0A%0A%0AVol-&_c=%238eb734%3B&=W%0A%0A%0A%0A%0A%0A%0AVol+&_c=%23f37201%3B&=V%0A%0A%0A%0A%0A%0A%0ABts-&_c=%23cf1d67%3B&=Z%0A%0A%0A%0A%0A%0A%0ABts+&_c=%23cccccc%3B&=Shift%3B&@=Ctrl&=Win&_a:7%3B&=&_a:4%3B&=Alt&_w:2%3B&=Space&_x:1&w:2%3B&=Enter&=Sym&=AltGr&=AltTab&=Ctrl)

### Usage
Program the Nyquist with QMK and use the keyboard with the OS's US-International layout with dead key support.

### Notes
- "Fun" is the function layer (function keys, navigation, and volume/brightness control).
- "Sym" is the symbol layer, similar to AltGr in the other layouts.
- The key "AltTab" enables Alt-Tabbing with just one keypress.
- The key "AltGr" is provided be able to use international characters via the OS's software layout.


## Linux

![Layout](https://github.com/xdlg/Dvorax/blob/master/linux/layout.png)

[Keyboard Layout Editor](https://www.keyboard-layout-editor.com/##@@=Esc&_c=%23cf1d67%3B&=!%0A1&_c=%23f37201%3B&=%2F@%0A2&_c=%238eb734%3B&=%23%0A3&_c=%2300548c%3B&=$%0A4&=%25%0A5%0A%0A%E2%82%AC&_c=%2300afef%3B&=(%5E)%0A6&=%2F&%0A7&_c=%238eb734%3B&=*%0A8&_c=%23f37201%3B&=(%0A9&_c=%23cf1d67%3B&=)%0A0&_c=%23cccccc&a:7%3B&=&=&_a:4&w:2%3B&=Backspace%3B&@_w:1.5%3B&=Tab&_c=%23cf1d67%3B&=(%22)%0A(')&_c=%23f37201%3B&=%3C%0A,%0A%0A(~)&_c=%238eb734%3B&=%3E%0A.%0A%0A(%60)&_c=%2300548c%3B&=P&=Y&_c=%2300afef%3B&=F&_fa@:0&:0&:0&:1%3B%3B&=G%0A%0A%0APgUp&_c=%238eb734%3B&=C%0A%0A%0A%2F&uarr%2F%3B&_c=%23f37201%3B&=R%0A%0A%0APgDn&_c=%23cf1d67%3B&=L&_f:3%3B&=%3F%0A%2F%2F%0A%7C%0A%5C&_c=%23cccccc&a:7%3B&=&_x:0.25&a:4&w:1.25&h:2&w2:1.5&h2:1&x2:-0.25%3B&=Enter%3B&@_w:1.75%3B&=AltGr&_c=%23cf1d67&f:3%3B&=A%0A%0A%0A%5B&_c=%23f37201&f:3%3B&=O%0A%0A%0A%5D&_c=%238eb734&f:3%3B&=E%0A%0A%0A%7B&_c=%2300548c&f:3%3B&=U%0A%0A%0A%7D&=I&_c=%2300afef%3B&=D%0A%0A%0AHome&=H%0A%0A%0A%2F&larr%2F%3B&_c=%238eb734%3B&=T%0A%0A%0A%2F&darr%2F%3B&_c=%23f37201%3B&=N%0A%0A%0A%2F&rarr%2F%3B&_c=%23cf1d67%3B&=S%0A%0A%C3%9F%0AEnd&_f:3%3B&=%2F_%0A-%0A+%0A%2F=&_c=%23cccccc&a:7%3B&=%3B&@_a:4&w:1.25%3B&=Shift&_a:7%3B&=&_c=%23cf1d67&a:4%3B&=%2F:%0A%2F%3B&_c=%23f37201%3B&=Q&_c=%238eb734%3B&=J&_c=%2300548c%3B&=K&=X&_c=%2300afef%3B&=B&=M&_c=%238eb734%3B&=W&_c=%23f37201%3B&=V&_c=%23cf1d67%3B&=Z&_c=%23cccccc&w:2.75%3B&=Shift%3B&@_w:1.25%3B&=Ctrl&_w:1.25%3B&=Win&_w:1.25%3B&=Alt&_a:7&w:6.25%3B&=&_a:4&w:1.25%3B&=AltGr&_w:1.25%3B&=Win&_w:1.25%3B&=Menu&_w:1.25%3B&=Ctrl)

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

[Keyboard Layout Editor](https://www.keyboard-layout-editor.com/##@@=Esc&_c=%23cf1d67%3B&=!%0A1&_c=%23f37201%3B&=%2F@%0A2&_c=%238eb734%3B&=%23%0A3&_c=%2300548c%3B&=$%0A4&=%25%0A5%0A%0A%E2%82%AC&_c=%2300afef%3B&=(%5E)%0A6&=%2F&%0A7&_c=%238eb734%3B&=*%0A8&_c=%23f37201%3B&=(%0A9&_c=%23cf1d67%3B&=)%0A0&_c=%23cccccc&a:7%3B&=&=&_a:4&w:2%3B&=Backspace%3B&@_w:1.5%3B&=Tab&_c=%23cf1d67%3B&=(%22)%0A(')&_c=%23f37201%3B&=%3C%0A,%0A%0A(~)&_c=%238eb734%3B&=%3E%0A.%0A%0A(%60)&_c=%2300548c%3B&=P&=Y&_c=%2300afef%3B&=F&=G&_c=%238eb734%3B&=C&_c=%23f37201%3B&=R&_c=%23cf1d67%3B&=L&=%3F%0A%2F%2F%0A%7C%0A%5C&_c=%23cccccc&a:7%3B&=&_x:0.25&a:4&w:1.25&h:2&w2:1.5&h2:1&x2:-0.25%3B&=Enter%3B&@_w:1.75%3B&=CapsLock&_c=%23cf1d67%3B&=A%0A%0A%0A%5B&_c=%23f37201%3B&=O%0A%0A%0A%5D&_c=%238eb734%3B&=E%0A%0A%0A%7B&_c=%2300548c%3B&=U%0A%0A%0A%7D&=I&_c=%2300afef%3B&=D&=H&_c=%238eb734%3B&=T&_c=%23f37201%3B&=N&_c=%23cf1d67%3B&=S%0A%0A%0A%C3%9F&=%2F_%0A-%0A+%0A%2F=&_c=%23cccccc&a:7%3B&=%3B&@_a:4&w:1.25%3B&=Shift&_a:7%3B&=&_c=%23cf1d67&a:4%3B&=%2F:%0A%2F%3B&_c=%23f37201%3B&=Q&_c=%238eb734%3B&=J&_c=%2300548c%3B&=K&=X&_c=%2300afef%3B&=B&=M&_c=%238eb734%3B&=W&_c=%23f37201%3B&=V&_c=%23cf1d67%3B&=Z&_c=%23cccccc&w:2.75%3B&=Shift%3B&@_w:1.25%3B&=Ctrl&_w:1.25%3B&=Win&_w:1.25%3B&=Alt&_a:7&w:6.25%3B&=&_a:4&w:1.25%3B&=AltGr&_w:1.25%3B&=Win&_w:1.25%3B&=Menu&_w:1.25%3B&=Ctrl)

### Usage
Open with Microsoft Keyboard Layout Creator, generate the installer, and install. The layout should appear as "German - Custom" or something similar.

### Notes
- Home row navigation keys aren't provided because KLC only supports them on the base layer.

