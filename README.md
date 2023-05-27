# makepkg-affinity
An Arch MakePKG to build Wine compatable with Affinity V2 suite

## On different distribution use toolbox and do the following:

### Prepare container
```
toolbox create --image quay.io/toolbx-images/archlinux-toolbox
toolbox enter archlinux-toolbox
git clone https://github.com/EnfrigFalco/makepkg-affinity.git
cd makepkg-affinity
sudo pacman -Sy nano

```
#### Enable multilib
```
sudo nano /etc/pacman.conf
```
    [multilib]
    Include = /etc/pacman.d/mirrorlist

### Build
makepkg
```
