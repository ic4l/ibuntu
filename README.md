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

## Install Composer



## Install Apache



## Install MySQL



## Install Compsoer
`sudo apt update`
`sudo apt install php-cli unzip`
`cd ~
curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php`
HASH=`curl -sS https://composer.github.io/installer.sig`
echo $HASH
php -r "if (hash_file('SHA384', '/tmp/composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
sudo php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer
`composer`

## If Error Installing Laravel (mkdir(): Permission denied)

`sudo chown -R $USER:$USER /var/www`
