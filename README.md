# ubuntu-settings

### googleChrome
sudo apt install gdebi-core wget

wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

sudo gdebi https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

### terminal bash to zsh
sudo apt install zsh

chsh -s /bin/zsh

### install vim
sudo apt install vim

### keyboard(keybinding)
https://qiita.com/kaleidot725/items/1eb4a2a4e47e9db01147

https://noumenon-th.net/programming/2018/11/10/ubuntu-us/

https://hirooka.pro/ubuntu-22-04-lts-japanese-input-ibus-fcitx-mozc/

### security
sudo apt install clamav
sudo apt install clamav-daemon

### emacs keybinding
gsettings set org.gnome.desktop.interface gtk-key-theme Emacs
