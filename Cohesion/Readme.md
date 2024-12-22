<p align="center">
  <img src="https://github.com/user-attachments/assets/b2dd7a25-a14a-4f0c-ad6c-bb8769e2e75c" alt="Wazz's custom image"/>
</p>

# Cohesion

A cohesive, transparent, and integrated style for [Zen Browser](https://zen-browser.app/)

https://github.com/user-attachments/assets/e19e1a3d-c3ea-42a1-a655-4b9353463ca5

### Install and Config
- Drop the Cohesion folder into your **chrome** folder
- Add `@import "Cohesion/Cohesion.css";` to the top of your **userChrome.css** file

Enable the following in `about:config`
- `browser.tabs.allow_transparent_browser` = `true`*
- `zen.view.use-deprecated-urlbar` = `true`
#### Known Issues:

*- Currently not compatible with [Zen Sidebar At Right Side](https://zen-browser.app/mods/dd4f5461-1564-4e56-9f9d-f81e3c18f93c).*

*- Currently not compatible with Collapsed Toolbar Mode.*

*- Some HDR displays render an incorrect Alpha value for certian elements, even though they are consistant within the userChrome.css file. This is believed to be a Windows HDR bug.*

*- Websites without a background will display the browser UI underneath the content.*

*(Extensions like [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/?utm_source=addons.mozilla.org&utm_medium=referral&utm_content=search) fix this by setting their own background.)*


