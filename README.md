# kbd-intl-ng

This repository contains improved international keyboard layouts for
Xorg, linuxs virtual console.

## usage

### tty

```
$ loadkeys us us-leah2-intl
```

### xorg

```
# setxkbmap -layout 'us(altgr-intl),de(nodeadkeys)' \
   -option 'grp:alt_shift_toggle,compose:menu'
# xmodmap ~/us-leah2-intl.xmodmap
```

## us-intl and us-altgr-intl

us-intl and us-altgr-intel are layouts based on Xorgs us(intl) and
us(altgr-intl), respectively.

## us-leah2-intl

This layout is based on
http://chneukirchen.org/dotfiles/.us-intl-german.xmodmap and extends Xorgs
us(intl) or us(altgr-intl) layouts.

CapsLock is used as additional modifier.

```
With CapsLock held these already do what they say if you press
them *as usual on the German* keyboard:
  ^ ä ö ü ß { [ ] } ! " § $ % & / ( ) = ? ` @ µ €

What this layout does is define these shortcuts, so you only need
group_switch:
  q@ e€ aä AÄ oö OÖ uü uÜ sß mµ 5€ 8( 9)

Additionally, we bind caps-hjkl to vi-style cursor keys, and HJKL to
Home, Next, Up, End.

Additionally, these typographic features:
. is ellipsis, shift-. is midpoint, alt-. is irony.
- is en-dash, shift-- is em-dash.
! is interrobang.
space is visible space, shift-space is nonbreaking space.
alt-s is long s, alt-y is ezh.
```
