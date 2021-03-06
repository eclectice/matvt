#### Please read the After Install instructions carefully otherwise you might end up soft-bricking yourself (it's possible to recover, but why do you want to risk it, eh?)

# MATVT: Mouse for Android TV Toggle

Hard to reach portions of some legacy app that you're running on your Android TV?
Feeling the need to have a touch input in your Android TV?
Or just looking for an alternative to the famous Mouse Toggle App for your TV?

MATVT solves all the above. Unfortunately, it's not on the playstore, and there are no plans to
launch it there either.

## So what does this app do?
MATVT is intended for users running Android TV (Android version 9+) and have a big remote with
atleast the following:
- DPAD (for up, down, left, right and center buttons)
- Color buttons (Red, Green, Yellow, Blue)
- Info button

After installing this app, you'll get a (*BIG*) mouse cursor that can move around, perform clicks and
left / right / up / down swipes from your remote itself without any extra hardware (no need to pair
with an android phone / laptop etc)

## How to install?
Download the APK from the releases section and side-load it on your TV.
The source-code is open and available should you wish to inspect it / build it yourself / don't
trust the release apk ;)

## How to use?
- DPAD is for movement and single clicks (I think I added long click support too, but isn't very reliable)
- The color buttons are for swiping. RED and GREEN for up/down swipe, YELLOW and BLUE for left/right swipe
- Info button will instantly toggle mouse visibility (so you can switch between mouse and no mouse instantly)
- Pressing back button for more than 3 seconds will disable the accessibility service completely
- The mouse will auto-disappear after a short while and re-appear when you press another relevant button.
- Toggling mouse visibility via the Info button resets cursor position
- The mouse warps around your TV sides, so you can roll over from the top of your TV to the bottom instantly
- Mouse movement is momentum based, so keeping key pressed for longer will increase the movement / send multiple swipes

# Important points to know After Installing
- Be sure to go to Special App Permissions in your settings and give permission to MATVT to draw over
other system apps. If you don't do this step and enable the accessibility service beforehand, the app won't have
necessary permissions to do anything and it'll keep consuming your input, so your remote will no longer work.
If you have gotten yourself in this situation, see FAQ.
- *AFTER* doing the above, you can go to accesibility settings and enable MATVT service.
- Now you can press the info button and there you have your mouse

# FAQs

- **Is this tested?**
  Yes, I have tested it on Sony Android TV. So any other Android TVs running Android 9 should work.

- **I didn't follow instructions properly and have soft-bricked myself, now what?**
  You'll need a physical mouse to go to accessibility services and disable MATVT. And this time before re-enabling it, please follow instructions and give the service proper permissions. You can also use a keyboard, but it'll be way more tedious.

- **I didn't follow instructions and was not soft-bricked, why all the warnings?**
  You should consider yourself lucky then :p. But be aware that the warnings are put there from a real experience.

- **So, how does it work?**
  You have the exact code in front of you, feel free to read it { It's not that bad ;) }. In a nutshell, this app uses Accessibility features provided by Android.

- **I think there's something that can be improved. How to contribute?**
  I welcome all kinds of contributions. Documentation, Code tests, Actual Hardware Testing etc etc. Please feel free to create a Pull request and remind me in a couple of weeks if I forget about it :D


# Credits
Thanks to EVA Facial Mouse for open sourcing their code. I've taken lots of ideas from their codebase. You can check them out at https://github.com/cmauri/eva_facial_mouse
