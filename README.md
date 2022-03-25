<h1 align="center">Notflix</h1>
<p align="center">Downloading torrents is old news, stream them with Notflix!</p>
<p align="center">Fork of notflix using older codebase</p>

<p align="center">
  <img src="./preview.gif" alt="Preview" width="500px">
</p>

## Installation
Dependencies:
* mpv
* WebTorrent
* dmenu

### Clone Method
If you'd like to download notflix in the 'traditional' way, then follow these steps.
* `$ git clone https://github.com/ayylmaonade/notflix`
* `$ cd notflix`
* `$ chmod +x notflix`
* `$ sudo cp notflix /usr/local/bin`

Optional: `$ rm -rf notflix` -- this removes the cloned repo as only the source notflix script is required.

### Using Curl
If you'd like to skip cloning and directly download just the script, then follow these steps.
* `$ sudo curl -sL "https://raw.githubusercontent.com/ayylmaonade/notflix/master/notflix" -o /usr/local/bin/notflix`
* `$ sudo chmod +x /usr/local/bin/notflix`

## Uninstall
You just need to simply remove the notflix script placed in /usr/local/bin
* `$ sudo rm /usr/local/bin/notflix` will completely remove the script.

## Usage
After installing, simply open a terminal and type notflix. The script will automatically run and prompt you to type what you wish to watch.

### Configuration
Notflix contains easily modifiable variables. For example, if you prefer a different tracker, you can change it from 1337x to whatever you please. They are as follows;
* `baseurl` -- this variable tells the script where to fetch results from. By default it is set to 1337x, but you may modify this so it defaults to your tracker of choice.
* `menu` -- this variable controls dmenu. By default it lists the top 25 seeded torrents with `menu="dmenu -i -l 25"` but this can be modified.
* `cachedir` -- this tells where notflix to write its cache. By default it's `cachedir="$HOME/.cache/notflix` although you can change this, it is **NOT** recommended. Only change this if you know what you're doing.
* If you'd like to change the default media player, you can remove `--mpv` and replace it with `--vlc` or any other flags of your choice. This is found at the bottom of the script.

All of these variables can be edited in your text editor of choice by opening the notflix script itself, making your changes, saving and ta-da! No extra steps required.

## License
This project is licensed under [GPL-3.0](https://raw.githubusercontent.com/Illumina/licenses/master/gpl-3.0.txt).

