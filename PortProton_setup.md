*Источник (Source): https://linux-gaming.ru/t/ustanovka-portproton-ispolzovanie-wine-proton-bez-steam/24*

# Alt Linux

```bash
su -
apt-get update && apt-get dist-upgrade -y
apt-get install portproton i586-{libvulkan1,libd3d,libGL,libgio,libnm,libnsl1,libnss,glibc-nss,glibc-pthread,libunwind,xorg-dri-swrast}
```

Вариант установки с помощью eepm: (Installation option using eepm:)

```bash
su -
epm full-upgrade
epm play portproton
```

# ROSA Linux

```bash
sudo urpmi portproton
```

# Ubuntu 24.04, Debian 12, Linux Mint 21.x, Deepin

```bash
dpkg --add-architecture i386
apt-get update
wget https://github.com/Castro-Fidel/PortProton_dpkg/releases/download/portproton_1.4-1_amd64/portproton_1.4-1_amd64.deb
apt install ./portproton_1.4-1_amd64.deb
```

# Arch Linux (Manjaro, Garuda...)

https://aur.archlinux.org/packages/portproton

# OpenSuse

https://software.opensuse.org/download/package?package=portproton&project=home%3ABoria138%3APortProton

# Fedora и Nobara

```bash
sudo dnf copr enable boria138/portproton
sudo dnf install portproton
```

# Fedora Silverblue, Fedora Kinoite и Bazzite

```bash
cd /etc/yum.repos.d
sudo wget  https://copr.fedorainfracloud.org/coprs/boria138/portproton/repo/fedora-$(rpm -E %fedora)/boria138-portproton-$(rpm -E %fedora).repo
sudo rpm-ostree install portproton
```

# flatpak version

```bash
flatpak install flathub portproton -y
```

https://flathub.org/apps/ru.linux_gaming.PortProton

Дополнительная информация (Additional Information [RU]): https://linux-gaming.ru/t/ustanovka-portproton-na-steamdeck/49
