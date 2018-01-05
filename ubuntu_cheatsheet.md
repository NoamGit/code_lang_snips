## Apps

### RESTART APPSTORE
$ killall gnome-software  
$ rm -r ~/.local/share/gnome-software

### UPDATE PYCHARM
[stackoverflow](https://stackoverflow.com/questions/23255033/update-pycharm-on-linux)

### [Uninstall intelliJ](https://askubuntu.com/questions/300684/uninstall-intellij-ultimate-edition-version-12/300692#300692)

### [install apps from tar](https://www.jetbrains.com/help/idea/install-and-set-up-intellij-idea.html)
```sh
sudo tar xf -*.tar.gz -C /opt/
```

## Common Issues

### LOGIN LOOP
[https://askubuntu.com/questions/760934/graphics-issues-after-while-installing-ubuntu-16-04-16-10-with-nvidia-graphics](https://askubuntu.com/questions/760934/graphics-issues-after-while-installing-ubuntu-16-04-16-10-with-nvidia-graphics "askubuntu link")  
$ sudo apt-get purge nvidia  
$ sudo apt-get install nvidia-{best suited version for graphics card 1050i TX}
