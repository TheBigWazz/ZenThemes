# Transparent New Tabs v2
Enable a blank, transparent, cohesive New Tab experience in [Zen Browser](https://zen-browser.app/) with this **Integrated URL Style**. 

Enjoy hints of your gradient behind the transparent URL bar or show it off completely in a New Tab!  

<p align="center">
  <img src="https://github.com/user-attachments/assets/9c862e82-d3e5-45d1-b1fb-6f2d75085b73" alt="Wazz's custom image"/>
</p>

## Set Up
- Set ```New Tab``` to ```Blank Page``` in **Zen Settings > Home > New Tab & Homepage**
  
  ![image](https://github.com/user-attachments/assets/a8586692-301b-4795-915b-7156b1eb87de)

- Set ```browser.tabs.allow_transparent_browser``` to ```true``` in **about:config**
 
  ![image](https://github.com/user-attachments/assets/bc419e92-0841-476f-b88b-ccd1be7750b7)

- Install [Dark Reader](https://addons.mozilla.org/en-US/firefox/addon/darkreader/) to auto set backgrounds on sites that don't have one already.
  
- Install [Drop Shadow](https://zen-browser.app/mods/abc2d6d8-ea9c-4313-a99c-fb1e76e8b3e5) mod to achieve the cohesive look between the Nav Bar and the Browser Container.
  
- Copy **userChrome.css** from this repo into *your* **userChrome.css** file

## Notes
### - Not compatible with custom homepages like Bonjourr or Tabliss -

The following mods break the cohesive appearance of the integrated URL style and it's recommended to disable them:
- [Cleaned URL bar]()

  -*Makes the URL bar too tall*
- [Sleek Borders]()
    
  -*Adds borders to Browser Container that break cohesive look*