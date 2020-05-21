# polybar-qbittorrent

[qBittorrent](https://github.com/qbittorrent/qBittorrent) module for [Polybar](https://github.com/jaagr/polybar)

![screenshot](screenshot.png)

## Dependencies

* [python3](https://www.python.org)
* Iosevka Nerd Font
* [qbittorrent-api](https://pypi.org/project/qbittorrent-api/)

## Usage

Modify `polybar-qbittorrent` file to match your qBittorrent config:

``` python
username=''
password=''
host='localhost'
port='8080'
```

By default, the module will not show if no torrent is active. Set `display_without_active` to `True` if you want to show it while no torrent is active

Make sure the `polybar-qbittorrent` is executable

``` bash
chmod +x polybar-qbittorrent
```

Use it in your polybar `config` as

``` yaml
[module/qbittorrent]  
type = custom/script  
exec = "/path/to/polybar-qbittorrent"  
interval = 0.1
````
