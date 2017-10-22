## Apps

### RESTART APPSTORE
$ killall gnome-software  
$ rm -r ~/.local/share/gnome-software

### UPDATE PYCHARM
[stackoverflow](https://stackoverflow.com/questions/23255033/update-pycharm-on-linux)

## Common Issues

### LOGIN LOOP
[https://askubuntu.com/questions/760934/graphics-issues-after-while-installing-ubuntu-16-04-16-10-with-nvidia-graphics](https://askubuntu.com/questions/760934/graphics-issues-after-while-installing-ubuntu-16-04-16-10-with-nvidia-graphics "askubuntu link")  
$ sudo apt-get purge nvidia  
$ sudo apt-get install nvidia-{best suited version for graphics card 1050i TX}