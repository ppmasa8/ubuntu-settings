# ubuntu-settings

### googleChrome
```bash
sudo apt install gdebi-core wget

wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

sudo gdebi https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```

### terminal bash to zsh
```bash
sudo apt install zsh

chsh -s /bin/zsh
```

### install vim
```bash
sudo apt install vim
```

### keyboard(keybinding)
https://qiita.com/kaleidot725/items/1eb4a2a4e47e9db01147

https://noumenon-th.net/programming/2018/11/10/ubuntu-us/

https://hirooka.pro/ubuntu-22-04-lts-japanese-input-ibus-fcitx-mozc/

### security
```bash
sudo apt install clamav

sudo apt install clamav-daemon
```

https://qiita.com/kannkyo/items/1cc32231afad88c11d8e

https://office54.net/iot/linux/ubuntu-cron-crontab#section1-2

### ssh
https://qiita.com/shizuma/items/2b2f873a0034839e47ce

### fix output device
```bash
sudo vim /etc/pulse/default.pa

…
### Should be after module-*-restore but before module-*-detect
load-module module-switch-on-port-available 

### Use hot-plugged devices like Bluetooth or USB automatically (LP: #1702794)
#.ifexists module-switch-on-connect.so　HERE comment out
#load-module module-switch-on-connect HERE
#.endif HERE
…
### Make some devices default
#set-default-sink output
#set-default-source input
```

### When no sound
```bash
sudo apt-get remove --purge pulseaudio
sudo apt-get install pulseaudio
mv ~/.config/pulse ~/.config/new_pulse_conf
```
After restart your PC.
