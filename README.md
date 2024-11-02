# ibuntu & Laravel
kumpulan command untuk setting Ubuntu & Laravel

## Merubah Login Screen untuk Primary Monitor 
`sudo cp ~/.config/monitors.xml /var/lib/gdm3/.config/`


## Membuat Permanent Alias
`sudo nano ~/.bashrc`
- Tambahkan command dibawah '# some more ls aliases'
`alias htdocs='cd /var/www/html'`
`alias iserve='php artisan serve --host ic4linux.local'`
`alias xsip='ssh -p 65002 u337986536@154.41.240.43'`

- Control + X .... Y untuk save and exit
- Jalankan command dibawah ini untuk refresh
  
`source ~/.bashrc`

## Install Brave Browser
`sudo apt install curl`

`sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg`

`echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] https://brave-browser-apt-release.s3.brave.com/ stable main"|sudo tee /etc/apt/sources.list.d/brave-browser-release.list`

`sudo apt update`

`sudo apt install brave-browser`

## Pre-requisite
- install web server di komputer
- `sudo apt install php libapache2-mod-php`
- install curl
- `sudo apt install curl php-cli php-mbstring git unzip php-curl`
- Install composer melalui CURL (Recomended)
- `curl -sS https://getcomposer.org/installer |php`
- `sudo mv composer.phar /usr/local/bin/composer`
- `sudo service apache2 restart`
- Install component yang dibutuhkan untuk COMPOSER
- `sudo apt install curl php-cli php-mbstring git unzip php-curl`
- `sudo apt-get install -y php8.*-gd`
- `sudo apt-get install php8.*-intl`
- `sudo apt-get install php8.*-xsl`
- `sudo apt-get install php8.*-mbstring`


## Install Apache



## Install MySQL


## Install PHPMyAdmin
`sudo apt install phpmyadmin`



## Install Composoer
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


## config/database.php ada di dalam folder project laravelnya
- Edit Strict

## QRCode for Laravel
`https://github.com/SimpleSoftwareIO/simple-qrcode/tree/develop/docs/en`
