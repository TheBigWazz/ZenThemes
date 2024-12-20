# My Personal CSS for Zen

Below are my customizations, mods, toolbar layout, extensions, and theme colors.

**I have only tested this exact set up on Windows 11.*

https://github.com/user-attachments/assets/1e880c38-5c36-4667-9d56-2ac59b9aaaff

## Step-by-step

__1.__ : [Zen Settings](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#Zen-Settings)

__2.__ : [about:config](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#aboutconfig-options)

__3.__ : [Toolbar Layout](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#toolbar-layout)

__4.__ : [Extensions](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#extensions)

__5.__ : [Install with uCL](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#userchromecss)

__6.__ : [userContent.css](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#usercontentcss)

__7.__ : [Mica For Everyone](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#mica-for-everyone)

__8.__ : [Mods](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#mods)

__9.__ : [Gradients](https://github.com/TheBigWazz/ZenThemes/tree/main/Zen-current-theme#gradients)

## 1. Zen Settings

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

## 2. About:Config Options

### Zen Options:

- ```browser.tabs.allow_transparent_browser``` = ```true```
  - *Allows transparency**

- ```zen.workspaces.show-workspace-indicator``` = ```false```
  - *Hide the Workspace Indicator*

- ```zen.view.use-deprecated-urlbar``` = ```true```
  - *Use the Connected URL style instead of Floating*

>[!Note]
>**Websites without a background will display the browser UI underneath the content.*
>
>*Extensions like [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) fix this by setting their own background.*

---

### Natsumi Tweaks Options:
*These options need to be manually added in `about:config`*

- ```natsumi.theme.clip-path-force-polygon``` = ```true```
  - *Uses polygon instead of inset for URLbar and Zen Sidebar blurring. Enable if you need this for compatibility with other userchromes/Mods*

- ```natsumi.sidebar.blur-zen-sidebar``` = ```true```
  - *Blurs Zen Sidebar background. This may cause some lag when you have both Zen Sidebar and Natsumi URLbar opened at the same time*

- ```natsumi.sidebar.containers-no-inactive-border``` = ```true```
  - *Hides the container tabs indicator border when the tab is not selected*

> [!WARNING]
> The developer of Zen Browser recommends **against** using custom CSS to implement Tab Groups like
> Natsumi's for the time being. Proceed at your own risk.
>
>- ```natsumi.sidebar.enable-tab-groups``` = ```true```
>   - *Enables Natsumi Tab Group Style*
>
>- `browser.tabs.groups.enabled` = ```true```
>   - *Enable Tab Groups*

---

## 3. Toolbar Layout

- Right click on the Tab Bar and select 'Customize Toolbar'
- Click and drag items to arrange them in this same order:

![image](https://github.com/user-attachments/assets/bf7919db-9e69-4aa5-8bfb-2a21d8da7813)

```[Account]```-```[Bookmark toolbar items]```-```[Proton Pass]```-```[4x Spacers]```-```[Nav buttons]```-```[URL Bar]```-```[Copy URL button]```-```[4x Spacers]```

## 4. Extensions
* [Copy Tab URL](https://addons.mozilla.org/en-US/firefox/addon/zen-copy-tab-url/) *Adds the Copy URL button to the URL bar.*
* [Proton Pass](https://addons.mozilla.org/en-US/firefox/addon/proton-pass/) *Is the purple diamond at the far left of the URL bar.*
* [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) *Fixes missing backgrounds on websites.*

## 5. Install with uCL
### What is uCL?
- [uCL (userChrome-Loader)](https://github.com/greeeen-dev/userchrome-loader) is an alternitive method of structuring custom CSS to make it easier for users to swap in and out specific Modules of code from the community. This method is more similar to how Zen Browser already structrues its Mods. In addition to being a simpler setup process, it's a much easier structure to debug and maintain. 

- Using uCL Structure allows an end user to simply drop a Mod folder into their **\chrome** folder to install a mod. 

- Instead of copying the entire CSS of a mod into a userChrome.css file, the user only needs to add a single import line in their userChrome.css.

- Mod creators can take advantage of this by making their custom css projects modular. Only want one feature of a project? Only use the import statement for that particular module. 

### Instructions:

1. If you have not already, follow the [Zen Live Editing](https://docs.zen-browser.app/guides/live-editing) guide to first make your own userChrome.css file.

2. Download the **"Wazz"**, **"Cohesion"**, and **"natsumi-tweaks"** folders from above and drop them into your **"chrome"** folder. 

3. Add these import statements to your **userChrome.css**:
```
/* Personal Changes */
@import "Wazz/Wazz.css";

/* Cohesion */
@import "Cohesion/Cohesion.css";

/* Natsumi */
@import "natsumi-tweaks/natsumi-tweaks.css";
```


> [!Note]
> - Remove any of my personal CSS / Cohesion CSS from your **userChrome.css** file if you have previously used it.
> - It's now all being called via the `@import "Wazz/Wazz.css";` statement in your **userChrome.css** file.
> - You may still add custom CSS to your userChrome.css underneath the imports.
> - You can Live Edit mod files, just search for the Module name in the Style Browser (Ctrl+Alt+Shift+I)

### What it does:
*Community contributions are credited inside the Modules.*

- Hides Pinned Tab Reset Button
- Styles Workspace Buttons
- URL Bar Loading animation
- Mini Container icon in URL (dot instead of full icon)
- [Cohesion](https://github.com/TheBigWazz/ZenThemes/tree/main/Cohesion) Mod
- [Natsumi](https://github.com/greeeen-dev/natsumi-browser/) Tweaks

> [!Note]
> Thanks to uCL structure, if you want to disable any of the features, simply remove the corresponding import statement from **"Wazz.css"**

## 6. userContent.css

### Instructions:

- Inside the same __"chrome"__ folder that your userChrome.css file is in, save '__[userContent.css]()__'
- Inside the same __"chrome"__ folder, save '__[zen-logo.svg]()__'

### What it does:

*By **@nova17_** on Discord*

- Adds Zen Logo on New Tab page, Home page, Blank Page, and Private Browsing page
- Adds transparency on New Tab Page/Firefox Home page

I made a tweak to remove the search bar from Firefox Home because I favor using the URL bar instead.

If you want the search bar back in Firefox Home, delete line 77 from **userContent.css**

![image](https://github.com/user-attachments/assets/eb8f90a8-5b31-465d-a104-a4329655b3da)

## 7. Mica For Everyone

- Download and install from their repo: https://github.com/MicaForEveryone/MicaForEveryone
- After installing, open and click the '__+__' button in the bottom left corner
- Click '__Add Process Rule__'
- Type ```zen```


## 8. Mods
These are all the mods I use:

* [Natsumi](https://github.com/greeeen-dev/natsumi-browser/) - [Natsumi Tweaks for Cohesion](https://github.com/TheBigWazz/ZenThemes/tree/main/natsumi-tweaks)
* [Cohesion](https://github.com/TheBigWazz/ZenThemes/tree/main/Cohesion)
* [Bottom Essentials](https://zen-browser.app/mods/477bc813-c333-4747-813e-00e0420ceec0)
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
  * Centeres the text inside the URL Bar: ```Always Centered```
  * Enable a background blur when the URL bar is focused & select its intensity: ```Really Strong```
  * [x] Always open websites in a new tab when using url bar

## 9. Gradients

![image](https://github.com/user-attachments/assets/fb165906-7601-4421-8a52-40b8dc3441e9)

![image](https://github.com/user-attachments/assets/db37488d-a723-41d2-9ff2-ff7e21459608)
