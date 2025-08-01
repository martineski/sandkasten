# Bluetooth Issues in PopOs

* **Description**: bluetooth toggle from the PopOs Settings menu is no longer available. Essentially, you can't turn bluetooth on anymore! This is annoying.

* [Useful Link](https://www.linux.org/threads/troubleshooting-bluetooth.55836/)

```sh
# help to see bluetooth chip in system
lsusb | grep -i blue
# see status of bluetooth
sudo systemctl status bluetooth
#
sudo systemctl enable bluetooth
sudo systemctl start bluetooth
sudo service bluetooth restart
```

* Another combination to try out:

```sh
rfkill list bluetooth
sudo systemctl restart bluetooth
sudo service bluetooth restart
```
