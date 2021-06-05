# Quietfox for Proton
Quietfox release for Proton, upgrades and improvments from myself, and from the Lepton project

## [Original](https://github.com/coekuss/quietfox)

## Designed to make Firefox feel better once again.

After proton, things broke, themes were lost, and tons of bad stuff happened. Thankfully, the quietfox theme was honestly minimally affected, and I decided to adapt it to use with my own system.

This theme was designed with Compact mode in mind, although Normal and Touch density can still be used.

## Features and Screenshots

### Tab Bar

![Screen Shot 2021-06-04 at 8 07 44 PM](https://user-images.githubusercontent.com/19739712/120878337-45705000-c5ab-11eb-9c52-1bab04036e79.png)

### Popout

![Screen Shot 2021-06-04 at 8 09 30 PM](https://user-images.githubusercontent.com/19739712/120878368-80728380-c5ab-11eb-868e-0d957b8743b2.png)

### Menus

![Screen Shot 2021-06-04 at 8 10 13 PM](https://user-images.githubusercontent.com/19739712/120878379-92ecbd00-c5ab-11eb-9043-9369ca90f200.png)


## Known Issues

### UNTESTED ON WINDOWS!!!

This theme is untested on Windows (I only have MacOS and Linux), if you encounter any errors, please open an issue!

### Transparent Themes

These screenshots were taken using the [Google Chrome Light Theme](https://addons.mozilla.org/en-US/firefox/addon/google-chrome-light/) theme, transparent themes such as Alpenglow look really bad:

![Screen Shot 2021-06-04 at 8 12 29 PM](https://user-images.githubusercontent.com/19739712/120878449-068eca00-c5ac-11eb-8b17-0cf4c797c961.png)

#### The Fix

In order to fix this, change the `--tab-corner-rounding` from `7px` to `0px`, and also follow the Dark Themes fix below.

```css
* { 
/* -------------------- 🎨 Customization 🎨 -------------------- */
    --tab-corner-rounding: 0px;
    --button-corner-rounding: 4px;
    --animation-speed: 0.15s;
}
```

### Dark Themes

In order to fix an issue with the title bar, the full URLbar was made white fix this in UserChrome by replacing 

```css
/* style address bar */
#urlbar-background {
    background-color: white !important;
    border: none !important;
/*     box-shadow: none !important; - Visual Diffrentiator*/
}
```

with 

```css
/* style address bar */
#urlbar-background {
    background-color: transparent !important;
    border: none !important;
/*     box-shadow: none !important; - Visual Diffrentiator*/
}
```

### Themes that have a differnet Tab color from the bar

Many themes such as the default light and dark ones, have a different tab color than the actual bar color, this messes up the theme and results in ugly colors like this:

![image](https://user-images.githubusercontent.com/19739712/120882315-58444e00-c5c6-11eb-9167-ba1c4dc7f11e.png)

For obvious reasons, themes need to have the same tab color as the bar color, as the two are visually connected!

The recommended theme is [Google Chrome Light](https://addons.mozilla.org/en-US/firefox/addon/google-chrome-light/).

### Accessibility

Unfortunatly, much like Proton, this theme is not made with Accessibility and contrast in mind, and more just for beauty. Feel free to make edits, but right now the only solution is listed [here](https://www.mozilla.org/en-US/firefox/all/#product-desktop-esr)

# Installation

1. Download the file from Releases
2. [Create a Chrome Folder](https://www.userchrome.org/how-create-userchrome-css.html)
3. Use the UserChrome from Releases rather than creating a new one.
4. Modify and Hack away!

Made with ❤️
