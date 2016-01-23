# yai3
(yet another i3)  
configs collection for borderless i3wm setup

## setup
* clone & copy
  ```
  git clone git@github.com:yacuken/yai3.git ~/yai3 && cd $_
  cp -R .config/* ~/.config
  cp -R .themes/* ~/.themes
  ```
* install stylish from stylish dir

## auto reloading styles in firefox
* install [custom buttons](https://addons.mozilla.org/ru/firefox/addon/custom-buttons/) extension (read description)
* create new button with code below
  ```
  var prefs = Components.classes["@mozilla.org/preferences-service;1"].getService(Components.interfaces.nsIPrefBranch).prefHasUserValue("extensions.stylish.styleRegistrationEnabled");
  if (prefs){
     stylishOverlay.turnOnOff(true);
  } else {
     stylishOverlay.turnOnOff(false);
  }
  ```
* edit [~/.config/dmenu/dmenu_themes:10](https://github.com/yacuken/yai3/blob/master/.config/dmenu/dmenu_themes#L10) with your shortcut

![http://www.youtube.com/watch?v=1dkNKHGdoys](./yai3_anim.gif)
*gif was edited*
