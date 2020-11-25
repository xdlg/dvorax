# Dvöraque

Dvorak keyboard layout with German and French character support

![Layout](https://github.com/xdlg/Dvorax/blob/master/layout.png)

[Keyboard Layout Editor](http://www.keyboard-layout-editor.com/##@@_a:7%3B&=&_c=%23cf1d67&a:4%3B&=!%0A1%0A%0A%0A%0A%0A%0A%0A%0A%0A%5B&_c=%23f37201%3B&=%2F@%0A2%0A%0A%0A%0A%0A%0A%0A%0A%0A%5D&_c=%238eb734%3B&=%23%0A3%0A%0A%0A%0A%0A%0A%0A%0A%0A%7B&_c=%2300548c%3B&=$%0A4%0A%0A%0A%0A%0A%0A%0A%0A%0A%7D&=%25%0A5%0A%0A%0A%0A%0A%0A%0A%0A%0A%C2%B0&_c=%2300afef%3B&=%5E%0A6%0A%0A%0A%0A%0A%0A%0A%0A%0A~&=%2F&%0A7%0A%0A%0A%0A%0A%0A%0A%0A%0A%60&_c=%238eb734%3B&=*%0A8&_c=%23f37201%3B&=(%0A9&_c=%23cf1d67%3B&=)%0A0&_c=%23cccccc&a:7%3B&=&=&_a:4&w:2%3B&=Backspace%3B&@_w:1.5%3B&=Tab&_c=%23cf1d67%3B&=%22%0A'&_c=%23f37201%3B&=%3C%0A,&_c=%238eb734%3B&=%3E%0A.&_c=%2300548c%3B&=P&=Y&_c=%2300afef%3B&=F&=G&_c=%238eb734%3B&=C%0A%0A%C3%87&_c=%23f37201%3B&=R&_c=%23cf1d67%3B&=L&=%3F%0A%2F%2F%0A%0A%0A%0A%0A%0A%0A%7C%0A%0A%5C&_c=%23cccccc&a:7%3B&=&_x:0.25&a:4&w:1.25&h:2&w2:1.5&h2:1&x2:-0.25%3B&=Enter%3B&@_w:1.75%3B&=Caps%20Lock&_c=%23cf1d67%3B&=A%0A%0A%C3%84&_c=%23f37201%3B&=O%0A%0A%C3%96&_c=%238eb734%3B&=E%0A%0A%0A%E2%82%AC&_c=%2300548c%3B&=U%0A%0A%0A%C3%9C&=I&_c=%2300afef%3B&=D&=H&_c=%238eb734%3B&=T&_c=%23f37201%3B&=N&_c=%23cf1d67%3B&=S%0A%0A%0A%C3%9F&=%2F_%0A-%0A%0A%0A%0A%0A%0A%0A+%0A%0A%2F=&_c=%23cccccc&a:7%3B&=%3B&@_a:4&w:1.25%3B&=Shift&_a:7%3B&=&_c=%23cf1d67&a:4%3B&=%2F:%0A%0A%0A%0A%0A%0A%2F%3B&_c=%23f37201%3B&=Q&_c=%238eb734%3B&=J&_c=%2300548c%3B&=K&=X&_c=%2300afef%3B&=B&=M&_c=%238eb734%3B&=W&_c=%23f37201%3B&=V&_c=%23cf1d67%3B&=Z&_c=%23cccccc&w:2.75%3B&=Shift%3B&@_w:1.25%3B&=Ctrl&_w:1.25%3B&=Win&_w:1.25%3B&=Alt&_a:7&w:6.25%3B&=&_a:4&w:1.25%3B&=AltGr&_w:1.25%3B&=Win&_w:1.25%3B&=Menu&_w:1.25%3B&=Ctrl)

## Linux

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
4. Log out and log back in.

Note that it's the `evdev` files that are modified, not the `base` or the `xfree86`. It's probably system-dependent, but at least on Linux Mint 19.3 Cinnamon only changing the `evdev` files worked out as desired.

After that, the layout should be available in the system preferences like any other language.
