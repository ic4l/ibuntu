# ibuntu
kumpulan command untuk setting ubuntu

## Merubah Login Screen untuk Primary Monitor 
`sudo cp ~/.config/monitors.xml /var/lib/gdm3/.config/`


## Membuat Permanent Alias
`sudo nano ~/.bashrc`
- Tambahkan command dibawah '# some more ls aliases'
  
`alias htdocs='cd /var/www/htdocs'`
- Control + X .... Y untuk save and exit
- Jalankan command dibawah ini untuk refresh
  
`source ~/.bashrc`

## Install Brave Browser
`sudo apt install curl`

`sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg`

`echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] https://brave-browser-apt-release.s3.brave.com/ stable main"|sudo tee /etc/apt/sources.list.d/brave-browser-release.list`

`sudo apt update`

`sudo apt install brave-browser`
