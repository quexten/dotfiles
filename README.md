# Quexten's Dotfiles

* **WM** i3-gaps
* **Compositor** Compton-Blur
* **Bar** Polybar
* **Launcher** Rofi
* **Shell** oh-my-zsh
* **Terminal** Konsole
* **Browser** Chromium-VAAPI

# Installation
```
git clone https://github.com/quexten/dotfiles.git
```

## Auto updating

I made a websocket endpoint available publishing a message every time this repo gets updated.
Automatically pull the changes like this:

### Using websocat

```
websocat - autoreconnect:ws://node-red-quexlabs.herokuapp.com/ws/github/dotfiles | while read -r line; do cd ~/dotfiles; git pull; done
```
