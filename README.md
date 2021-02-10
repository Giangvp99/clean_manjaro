#Clean pkg cache 

list packages
  ls /var/cache/pacman/pkg/ | less

Remove packages except those installed
  sudo pacman -Sc




#Remove unused packages

List unused
  sudo pacman -Qtdq

Remove unused
  sudo pacman -R $(pacman -Qtdq)
