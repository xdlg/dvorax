
# Dvorax

Somewhat symmetrical ISO 105 keyboard layout based on Dvorak, with German and French character support

![Layout](https://github.com/xdlg/Dvorax/blob/master/layout.png)

[Keyboard Layout Editor](http://www.keyboard-layout-editor.com/##@@_c=%23cf1d67%3B&=%7B%0A%5B&=(%0A4&=!%0A3&_c=%23f37201%3B&=%2F@%0A2&_c=%238eb734%3B&=%23%0A1&_c=%2300548c%3B&=$%0A0&_c=%23cccccc%3B&=%5E%0A~&_c=%2300afef%3B&=%2F&%0A5&_c=%238eb734%3B&=*%0A6&_c=%23f37201%3B&=+%0A7&_c=%23cf1d67%3B&=%2F=%0A8&=)%0A9&=%7D%0A%5D&_w:2%3B&=Backspace%3B&@_w:1.5%3B&=Tab&=%22%0A'&_c=%23f37201%3B&=%3C%0A,&_c=%238eb734%3B&=%3E%0A.&_c=%2300548c%3B&=P&=Y&_c=%2300afef%3B&=F&=G&_c=%238eb734%3B&=C%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%C3%87&_c=%23f37201%3B&=R&_c=%23cf1d67%3B&=L&=%3F%0A%2F%2F&=%7C%0A%5C&_x:0.25&w:1.25&h:2&w2:1.5&h2:1&x2:-0.25%3B&=Enter%3B&@_w:1.75%3B&=Backspace&=A%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%C3%84&_c=%23f37201%3B&=O%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%C3%96&_c=%238eb734%3B&=E%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%E2%82%AC&_c=%2300548c%3B&=U%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%C3%9C&=I&_c=%2300afef%3B&=D&=H&_c=%238eb734%3B&=T&_c=%23f37201%3B&=N&_c=%23cf1d67%3B&=S%0A%0A%0A%0A%0A%0A%0A%0A%0A%0A%C3%9F&=%2F_%0A-&=%C2%B0%0A%25%3B&@_w:1.25%3B&=Shift&=%2F:%0A%2F%3B&_c=%23f37201%3B&=Q&_c=%238eb734%3B&=J&_c=%2300548c%3B&=K&=X&_c=%23cccccc%3B&=%60%0A%C2%B4&_c=%2300afef%3B&=B&=M&_c=%238eb734%3B&=W&_c=%23f37201%3B&=V&_c=%23cf1d67%3B&=Z&_w:2.75%3B&=Shift%3B&@_c=%23cccccc&w:1.25%3B&=Ctrl&_w:1.25%3B&=Win&_w:1.25%3B&=Alt&_a:7&w:6.25%3B&=&_a:4&w:1.25%3B&=AltGr&_w:1.25%3B&=Win&_w:1.25%3B&=Menu&_w:1.25%3B&=Ctrl)

## Background

Strict touch typing on a standard keyboard (i.e. row-staggered) makes absolutely no sense for the left hand. Look at the standard areas of responsibility for each finger:

![Touch typing](https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/Touch_typing.svg/1200px-Touch_typing.svg.png)The right hand is fine, as the top-left to bottom-right key alignment (for example 7, U, J, M) matches the natural movement of the fingers. The hand can be kept in alignment with the forearm, and the wrist at a neutral angle.

The left hand is *not* fine, as the key alignment runs counter to the finger movement. You either have to bend your wrist inward or make some finger contortions, especially for the bottom row. For example, reaching down from A to Z with your pinky while keeping a neutral wrist angle is an extremely awkward movement. I believe that most people choose to bend their wrists inwards, which sounds and feels like a sure way to get RSI.

The culprit is row staggering, inherited from typewriters. Keyboards like the [X-Bows](https://x-bows.com/) or the [Ergodox](https://ergodox-ez.com/) address that problem, but they're still expensive, and I like the frugality of a software solution.

## Characteristics

Dvorax is a somewhat symmetrical keyboard layout based on Dvorak. It takes advantage of the ISO 105 keyboard to shift the left half of the bottom row one key to the left. The home row and the top row stay the same. Reaching the top row with neutral wrists isn't a problem for me, as the staggering is much less pronounced than with the bottom row. We won't achieve perfect symmetry on a  standard keyboard anyway.

![Layout](https://github.com/xdlg/Dvorax/blob/master/layout.png)

Additional characteristics:
- The layout should be usable on Linux and Windows. So features that could be programmed with xkb or xmodmap but not Microsoft Keyboard Layout Creator are out.
- I mostly write in English, often in German and occasionally in French, so I want good support for German characters and decent support for French characters.
- Leaving the 0 and 1 on the weakest fingers makes no sense, as they are by far the most important digits. Also, having the 0 completely to the right always seemed weird to me. In Dvorax, the 0 and 1 are on strong fingers, and the digit progression is mirrored.
- Parentheses, brackets, and curly brackets are symmetrical.
- Moving half the bottom row to the left and reorganizing the digits row leaves an empty key on each. These keys are the least reachable for either hand, so they be assigned to characters used only occasionally.
- The other special characters are mostly taken from Dvorak.
- I don't need Caps Lock, so it is now an additional Backspace.

# Linux

I use Linux Mint so installation steps may vary on other distributions. I chose xkb rather than xmodmap because it creates a layout that is completely integrated into the OS's preferences, just like any other language layout.

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

# Resources

 - [Xah Lee](http://www.xahlee.info/kbd/keyboard_blog.html) has a ton of information on keyboards
 - [SymmeTri](https://github.com/WesleyBlancoYuan/SymmeTri-Keyboard-Layout) and [The Symmetric Typing Project](http://kennetchaz.github.io/symmetric-typing/) are other attempts at symmetrical layouts
 - [The standard QWERTY finger placement is uncomfortable and terribly designed.](http://www.onehandkeyboard.org/standard-qwerty-finger-placement/)
