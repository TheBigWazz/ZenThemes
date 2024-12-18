# Cohesion Compatible Tweaks
These are the changes I made to Natsumi to make it more compatible with Cohesion, along with some personal style preferences.
- Corrected browser border values
- Changed URL animation timings
- Changed URL Input font size
- Removed border from non-selected Container Tabs

*Visit: https://github.com/greeeen-dev/natsumi-browser to check out the unmodified version.*
---

<h1 align="center">
  <img width="120" height="120" src="https://github.com/greeeen-dev/natsumi-browser/blob/main/images/icon.png?raw=true">
  <br>
  Natsumi Browser
</h1>

<p align="center">A skin for Zen Browser that makes things <strong><i>~flow~</i></strong>.</p>

![](https://github.com/greeeen-dev/natsumi-browser/blob/main/images/natsumi-preview.png?raw=true)

## What is Natsumi Browser?
Natsumi Browser (or Natsumi, for short) is a userchrome made for [Zen
Browser](https://zen-browser.app) that adds lots of polish to the design by incorporating animations,
blurs and more. It's pretty much the userchrome I personally use, but made public.

Natsumi is NOT a standalone browser. I don't even intend on making one.

Natsumi has been tested on `1.0.2-b.2` (Beta) and `1.0.2-t.3` (Twilight).

## Features
### Polished look
Natsumi Browser's looks are based on asev's [ZenCss](https://github.com/lunar-os/ZenCss), with some
additional tweaks and patches added on top to create a beautiful and polished experience.

![](https://github.com/greeeen-dev/natsumi-browser/blob/main/images/interface.gif?raw=true)

### Natsumi URLbar
With Natsumi URLbar, Natsumi gives the expanded URLbar a completely fresh new look, so it feels very
cozy while also having lots of room for search suggestions.

![](https://github.com/greeeen-dev/natsumi-browser/blob/main/images/natsumi-urlbar.gif?raw=true)

### Tab Groups
Natsumi Browser uses a customized version of [vicky5124](https://github.com/vicky5124)'s CSS for Tab
Groups. Group away to keep things organized!

![](https://github.com/greeeen-dev/natsumi-browser/blob/main/images/tab-groups.gif?raw=true)

## Installation
This skin is not available on the Zen Mods page, as this isn't intended to be a Mod. You will need to
install it by applying the userChrome.css file to the browser.

Read the [guide for live editing Zen Browser](https://docs.zen-browser.app/guides/live-editing) for more
details.

## Browser configs (in about:config)
These are the configs you can use to tweak Natsumi Browser. If you want to tweak the animation duration
and delay, change the variables in the userChrome.css file.

### Base theme
- `natsumi.theme.disable-blur`: Disables blurring for Natsumi URLbar and Zen Sidebar. Use this if
  Zen Browser lags too much.
- `natsumi.theme.disable-loading-animations`: Disables loading animation for tabs.
- `natsumi.theme.disable-urlbar-animation`: Disables URLbar loading animation for tabs.
- `natsumi.theme.enable-border-animation`: Enables border loading animation for tabs. This may use up
  quite some GPU.
- `natsumi.theme.better-findbar-addon`: Enables some tweaks to
  [RobotoSkunk](https://github.com/RobotoSkunk)'s [Better Find
  Bar](https://zen-browser.app/mods/a6335949-4465-4b71-926c-4a52d34bc9c0/) Mod.

### URLbar
- `natsumi.urlbar.disabled`: Disables Natsumi URLbar and reverts the URLbar style back.
- `natsumi.urlbar.disable-transparency`: Disables URLbar background transparency.
- `natsumi.urlbar.force-nowrap`: Prevents wrapping to make things more compact regardless of window
  width.
- `natsumi.urlbar.light`: Disables some animations to make Natsumi URLbar lighter.

### Sidebar
- `natsumi.sidebar.blur-zen-sidebar`: Blurs Zen Sidebar background. This may cause some lag when you
  have both Zen Sidebar and Natsumi URLbar opened at the same time.
- `natsumi.sidebar.containers-dashed-border`: Uses dashed border for container tabs instead of solid
  border. Selected tabs will always use solid border.
- `natsumi.sidebar.containers-right-gradient`: Moves container tabs indicator gradient to the right.
- `natsumi.sidebar.containers-thicker-gradient`: Makes container tabs indicator gradient "thicker".
- `natsumi.sidebar.disable-bigger-tab-label`: Disables bigger tab labels and reverts them back to the
  normal font size.
- `natsumi.sidebar.disable-panel-transparency`: Disables transparent background for sidebar panels
  (e.g. Bookmarks).

### Misc
- `natsumi.debug.legacy`: Enables support for 1.0.2-b.0 and 1.0.2-b.1.

## Troubleshooting
### "URLbar blur won't work!"
Make sure both `layout.css.backdrop-filter.enabled` and `layout.css.backdrop-filter.force-enabled` are
set to true. Also make sure that you're using WebRender and hardware rendering.

### "Zen Browser lags a lot!"
This may be due to the URLbar blurring or animations (likely the blur). Set `natsumi.theme.disable-blur`
to false to disable the blur, and `natsumi.urlbar.light` to true to disable the animations.

### "I don't see any of the Natsumi options in about:config!"
These are custom options which you need to create. Type in the exact name, then press the plus button on
the right to create the config.

### "Tab groups aren't working!"
Set `browser.tabs.groups.enabled` to true.

## Acknowledgements
Thank you to:
- [asev](https://github.com/lunar-os) for ZenCss, which serves as the base for Natsumi Browser's base
  CSS, and the tab appear animation
- [vicky5124](https://github.com/vicky5124) for the Tab Groups CSS
- [mr-cheff](https://github.com/mr-cheff) and Zen's
  [contributors](https://github.com/zen-browser/desktop/graphs/contributors) for creating Zen Browser
