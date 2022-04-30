<h2 align="center">:white_flower: :heart: :cherry_blossom: :heart: :cherry_blossom: :heart: :cherry_blossom: Welcome! :cherry_blossom: :heart: :cherry_blossom: :heart: :cherry_blossom: :heart: :white_flower:</h2></br>
<img src="assets/WALL.png"></br>
<img src="assets/TILED.png"></br>
<img src="assets/ROFI.png"></br>

This is a collection of dotfiles which I use with bspwm. If you find something you like, take it and make it yours! :heart: </br>

Most of these files will work out of the box assuming you have the applications installed. The file structure is a replica of the expected $HOME structure so installing them is as simple as cloning and linking (or moving if you prefer but linking keeps all your configs in one place).

```
git clone https://github.com/Miusaky/bspdots.git $HOME
cp --remove-destination -as $HOME/bspdots/. $HOME/
```


<h3> Additional notes </h3>


* If you like the colour scheme you can find it [here](https://github.com/SAGAtheme/SAGA) and *some* pre-written themes [here](https://github.com/SAGAtheme/).
* Some bar modules require additional dependencies to work:
    * CPU modules require lm_sensors.
    * Pipewire (available but not enabled out of the box) require pamixer.
    * Update module require the xbps package manager (Void Linux). If you're on Arch you can install [this pkg](https://aur.archlinux.org/packages/checkupdates+aur) and replace the command in the config. 
    * VPN module (available not but enabled) require Mullvad but can be adapted to other providers.
    * Menus and VPN modules make use of rofi to some extent. 
    * GPU modules require an Nvidia card (and the their drivers).
* The rofi powermenu uses loginctl. If it doesn't work for you can replace all occurrences of it in powermenu.sh with systemctl. 
* The included .zshrc depends on the (also included) antigen file to automatically install plugins. Do not use one without the other. 
* If fonts are not rendering make sure you run `fc-cache -v` after linking the files. </br>
* I use [colorer](https://github.com/kiddae/colorer) to switch colour schemes. [SAGA] is the default palette and if you're satisfied with that you don't need to install colorer as long as you keep its config files ($HOME/.config/colorer). If you do want to test other colours there are quite a few included in $HOME/.config/colorer/flavours. To switch you need to install colorer and run `colorer $HOME/.config/colorer/flavours/schemename`. 
* Fonts, GTK theme and icons are included but you will have to switch to them (either in the gtk file or using something like lxappearance). Iosevka Term Heavy is my primary font. 
* The Firefox theme is not included but can be found [here](https://github.com/SAGAtheme/Firefox). </br>

That's all you need to replicate this setup. However if you're curious about what other software I use (and would recommend) you can find a list below. </br>

|  TYPE      |  NAME      |
|------------|------------|
| OS         | Void ♥️     |
| Shell      | Zsh        |
| Bar        | Polybar    |
| Temrinal   | Kitty      |
| Editor     | Helix & Neovim     |
| Compositor | Picom      |
| Launcher   | Rofi       |
| Browser    | Firefox    |
| Palette    | SAGA  ♥️    |


## ACKNOWLEDGEMENTS
- [Kiddae](https://github.com/kiddae) for the lovely tool that is colorer.
- [Siduck](https://github.com/siduck) for his amazing dotfiles which I used for inspiration (and at some point served as templates for mine). 
- [adi1090x](https://github.com/adi1090x) for the beautiful ncmpcpp config.



