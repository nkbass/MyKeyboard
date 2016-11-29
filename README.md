# MyKeyboard

an android software keyboard for Vim and Busybox sh.

* QWERTY layout keyboard for tablets.
* requires android 4.1.2 or more.
* developing with Android Studio 2.2.2.
* an etude. this is not usable now.

if you want finished keyboard, go to these pages.
* https://play.google.com/store/apps/details?id=jp.co.pline.android.ctrlkeyboard
* https://github.com/klausw/hackerskeyboard


do not use in ordinary text editor,
because this keyboard sends raw control characters to edit field.

i want to implement flick shift and flick ctrl,
but current implementation is shift lock and ctrl lock.

## to compile

1. open config dialog.
[menu] Run -> Edit Configurations...

2. set "Launch options" to "Nothing".
these codes have no activities.

## tools dir
* keys.awk
  keyboard layout xml tag generator awk script.
 ```sh
 awk -f keys.awk i-qwerty.txt
 ```