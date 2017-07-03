# speed up the shutdown process
## while shutdown , f2->'stopping thermal daemon/running fit make remote cups printers'
sudo systemctl stop cups-browsed.service
sudo systemctl disable cups-browsed.service

# excute shadowsocks.sh when start
add 'sh /home/cjl/chenningss.sh' before 'exit 0' in /etc/rc.local

# disable fading windows
in 'CompisConfig Settings Manager'(need python2 as default python, and 'sudo apt-get install compizconfig-settings-manager'), Effects>Fading Windows

# bing dynamic wallpapers
clone https://github.com/genzj/pybingwallpaper
pip install .
add bin/BingWallpaper to /etc/rc.local
