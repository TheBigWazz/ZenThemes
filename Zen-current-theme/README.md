# Current CSS Preview

Below are my customizations, mods, toolbar layout, extensions, and theme colors.

**This exact set up has only been tested/used on Windows 11.*

![image](https://github.com/user-attachments/assets/6cf3eba9-db78-41f1-8ea3-8d193d096f61)

## Step-by-step

Follow these steps if you want the same as the screenshot:

__Step 0__ : [Zen Settings](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#Zen-Settings)

__Step 1__ : [about:config](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#aboutconfig-options)

__Step 2__ : [Toolbar Layout](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#toolbar-layout)

__Step 3__ : [Extensions](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#extensions)

__Step 4__ : [userChrome.css](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#userchrome.css)

__Step 5__ : [userContent.css](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#usercontent.css)

__Step 6__ : [Mica For Everyone](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#mica-for-everyone)

__Step 7__ : [Mods](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#mods)

__Step 8__ : [Gradients](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#gradients)

## Zen Settings

- Look and Feel 
  - Select '__Multiple Toolbars__'
  - Uncheck '__Show New Tab Button on Tab List__'
  - Uncheck '__Show border for the bottom icons__'
  - Zen URL bar Behavior = Normal
- Tab Management
  - Check '__Hide the default container indicator in the tab bar__'
  - Check '__Allow workspaces have their own pinned tabs__'
  - Check '__Display workspaces as an icon strip__'
- Home 
  - Homepage and new windows: Firefox Home (default)
  - New tabs: Firefox Home (default)


## About:Config Options

Allow transparency:

```browser.tabs.allow_transparent_browser``` = ```true```*

Hide the Workspace Indicator:

```zen.workspaces.show-workspace-indicator``` = ```false```

Use the Connected URL style instead of Floating:

```zen.view.use-deprecated-urlbar``` = ```true```

**Websites without a background will display the browser UI underneath the content.*

*Extensions like [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) fix this by setting their own background.*

## Toolbar Layout

- Right click on the Tab Bar and select 'Customize Toolbar'
- Click and drag items to arrange them in this same order:

![image](https://github.com/user-attachments/assets/bf7919db-9e69-4aa5-8bfb-2a21d8da7813)

```[Account]```-```[Bookmark toolbar items]```-```[Proton Pass]```-```[4x Spacers]```-```[Nav buttons]```-```[URL Bar]```-```[Copy URL button]```-```[4x Spacers]```

## Extensions
* [Copy Tab URL](https://addons.mozilla.org/en-US/firefox/addon/zen-copy-tab-url/) *Adds the Copy URL button to the URL bar.*
* [Proton Pass](https://addons.mozilla.org/en-US/firefox/addon/proton-pass/) *Is the purple diamond at the far left of the URL bar.*
* [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) *Fixes missing backgrounds on websites.*

## userChrome.css

### Instructions:

If you have not already made your own, follow the [Zen Live Editing](https://docs.zen-browser.app/guides/live-editing) steps first to make your own userChrome.css file.

If you already have a userChrome.css file, copy and paste my [userChrome.css]() into yours. Remember to save. 

You can copy the entire file or specific parts. It's mostly labled so you should be able to pick out exactly what you want. 

### What it does:
*Community contributions are credited inside the file.*

- Hides Pinned Tab Reset Button
- Styles Workspace Buttons
- Styles Tab Groups and makes them Workspace specific
- Hides the workspace 
- URL Bar Loading animation
- Mini Container icon (dot)
- [Cohesion]() Mod

## userContent.css

### Instructions:

- Inside the same __\chrome__ folder that your userChrome.css file is in, save '__[userContent.css]()__'
- Inside the same __\chrome__ folder, save '__[zen-logo.svg]()__'

### What it does:

*By **@nova17_** on Discord*

- Adds Zen Logo on New Tab page, Home page, Blank Page, and Private Browsing page
- Adds transparency on New Tab Page/Firefox Home page
- I made a tweak to remove the search bar from Firefox Home because I favor using the URL bar instead

## Mica For Everyone

- Download and install from their repo: https://github.com/MicaForEveryone/MicaForEveryone
- After installing, open and click the '__+__' button in the bottom left corner
- Click '__Add Process Rule__'
- Type ```zen```


## Mods
These are all the mods I use:

* [Cohesion](https://github.com/TheBigWazz/ZenThemes/tree/main/Cohesion)
* [Bottom Essentials](https://zen-browser.app/mods/477bc813-c333-4747-813e-00e0420ceec0)
* [Better Active Tab](https://zen-browser.app/mods/d8b79d4a-6cba-4495-9ff6-d6d30b0e94fe)
* [Better Unloaded Tabs](https://zen-browser.app/mods/f7c71d9a-bce2-420f-ae44-a64bd92975ab)
* [Cleaner Extension Menu](https://zen-browser.app/mods/1e86cf37-a127-4f24-b919-d265b5ce29a0)
* [Cleaned URL Bar](https://zen-browser.app/mods/a5f6a231-e3c8-4ce8-8a8e-3e93efd6adec)
* [Floating Status Bar](https://zen-browser.app/mods/906c6915-5677-48ff-9bfc-096a02a72379)
* [Hide Extension Name](https://zen-browser.app/mods/cb15abdb-0514-4e09-8ce5-722cf1f4a20f)
* [Midnight](https://zen-browser.app/mods/5ca67725-1f43-4ff2-9fcf-0c59af71c73a)
* [Only Close On Hover](https://zen-browser.app/mods/4596d8f9-f0b7-4aeb-aa92-851222dc1888)
* [SuperPins](https://zen-browser.app/mods/ad97bb70-0066-4e42-9b5f-173a5e42c6fc)

  **SuperPins Settings:**
  * [x] Makes pinned tabs look similar to Essentials (icon only in a grid)
  * [x] Adds a background to the pinned tabs
  * Select the gap between Essentials: ```Normal```
* [Super URL Bar](https://zen-browser.app/mods/d93e67f8-e5e1-401e-9b82-f9d5bab231e6)

  **Super URL Bar Settings:**
  * [x] Adjusts the border radius of the url bar and its items
  * Centeres the text inside the URL Bar: ```Always Centered```
  * [x] Move 1 button that's directly next to the url bar (you can do that by using 'Customize Toolbar') into the url bar
  * Enable a background blur when the URL bar is focused & select its intensity: ```Really Strong```
  * [x] Always open websites in a new tab when using url bar

## Gradients

![image](https://github.com/user-attachments/assets/fb165906-7601-4421-8a52-40b8dc3441e9)

![image](https://github.com/user-attachments/assets/db37488d-a723-41d2-9ff2-ff7e21459608)