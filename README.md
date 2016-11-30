# MyKeyboard

an android software keyboard for Vim and Busybox sh.
this is an etude. **this is not usable** now.

* QWERTY layout keyboard for tablets.
* requires android 4.1.2 or more.
* making  with Android Studio 2.2.2.

do not use in ordinary text editor,
because this keyboard sends raw control characters to edit field.

i want to implement flick shift and flick ctrl,
but current implementation is shift lock and ctrl lock.

## reference

### official sample code of soft keyboard
https://android.googlesource.com/platform/development/+/master/samples/SoftKeyboard

### other soft keyboards
* https://github.com/klausw/hackerskeyboard
* https://play.google.com/store/apps/details?id=jp.co.pline.android.ctrlkeyboard

## to compile this code in Android Studio

1. open config dialog.
[menu] Run -> Edit Configurations...

2. set "Launch options" to "Nothing".
these codes have no activities.

## tool
* keys.awk
  keyboard layout xml tag generator.
 ```sh
 cd {path_to_this_project}/tool
 awk -f keys.awk i-qwerty.txt
 ```
