dm.
==============================
A dark theme for [rEFInd](http://www.rodsbooks.com/refind/) based on [Dream Machine](https://github.com/Lindstream/dm-refind-theme).
----
**Screenshot**
![M](https://github.com/wignut0011/dm-EmeraldDark/blob/master/screenshot.png)

This is a fork of [DM by mustaqimM](https://github.com/mustaqimM/dm) that follows the color scheme of CachyOS's Emerald Dark. I also added an icon for CachyOS along with a version that follows the original DM color scheme in /SVGs.

I also made this fork easy(ish) to change. I included two Photoshop files (I used [Photopea](photopea.com)) for the screenshot and background. The Hue adjustment layer is for the forground color elements while the Color Replace adjustment layer is for the background color. Just be sure to leave "colorize" enabled and don't touch "Fuzziness". They are located in /PSD-Edit-Files/

Installation
----
```
$root: cp -r ~/dm /boot/efi/EFI/refind/themes
$root: nvim + /boot/efi/EFI/refind/refind.conf # Opens nvim and puts the cursor on the last line
$root: # Append "include themes/dm-EmeraldDark/theme.conf" to `refind.conf`
```
__NOTES:__
If you downloaded this via .zip then make sure to remove "-master" in the extracted folder.

Obviously [rEFInd](http://www.rodsbooks.com/refind/) is needed to use this. Install with your package manager `refind-efi`. You many need to run `refind-install` afterwards.

If the `refind` bootloader doesn't show up on boot even after running `refind-install`. Run `efibootmgr` (to see the current boot order), then set the order so it is loaded first, for example: `efibootmgr -o 0002,0003,0001`. You may first need to clear the boot order: `efibootmgr -O` OR delete a specific entry: `efibootmgr -A 0002`

----  
Attributions
----

**Font:** [Dento font](http://fontmeme.com/freefonts/34867/dento.font)

**Icons:** [Lightness for burg](http://sworiginal.deviantart.com/art/Lightness-for-burg-181461810) & [refind-ambience](https://github.com/lukechilds/refind-ambience).

**Reddit:** [rEFInd](http://www.rodsbooks.com/refind/)

----
