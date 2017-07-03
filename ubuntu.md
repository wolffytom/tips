# speed up the shutdown process
## while shutdown , f2->'stopping thermal daemon/running fit make remote cups printers'
sudo systemctl stop cups-browsed.service
sudo systemctl disable cups-browsed.service
