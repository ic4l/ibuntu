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
