# Free vps 6 jam linux ubuntu 20.04 2 core 4GB RAM
tutorial lengkap https://www.youtube.com/watch?v=BzWwuYL3-IU
 
## jalankan xface mining di paper space
 
## mining lewat web mining https://miner.nimiq.com/
 
## https://console.paperspace.com/login
 ```
 sudo apt update
```
```
sudo apt-get install gnome-panel gnome-settings-daemon metacity nautilus gnome-terminal
```
```
sudo apt install -y tightvncserver nano net-tools
```
```
sudo vncserver
```

```
sudo nano ~/.vnc/xstartup
```
 
Add the following lines to the file.
```
gnome-panel &
gnome-settings-daemon &
metacity &
nautilus &
```
Lalu disimpan
```
sudo vncserver -kill :1
```

```
sudo vncserver
```

```
sudo apt install novnc
```

```
websockify -D --web=/usr/share/novnc/ --cert=/etc/ssl/novnc.pem 6080 localhost:5901
``` 
## install chrome 
```
sudo wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```

```
sudo apt install ./google-chrome-stable_current_amd64.deb
```
 
## ubah  /usr/bin/google-chrome 
```
sudo nano  /usr/bin/google-chrome
```
baris terakhir isi dengan :
```
--no-sandbox
```
Nanti hasilnya akan seprti ini :
## exec -a "$0" "$HERE/chrome" "$@" --no-sandbox
 
## koneksikan vps dengan cloudflare melalui zero tier
Cek ip dari vps nya ketik :
```
ifconfig
```

Selengkapnya lihat https://www.youtube.com/watch?v=BzWwuYL3-IU mulai menit ke 16:25
 
