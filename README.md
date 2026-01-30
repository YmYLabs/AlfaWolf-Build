# AlfaWolf Linux Build Repository.

## Nasıl yapılır?

### Gerekli uygulamaları yükleme.

```
sudo apt update && sudo apt upgrade -y
sudo apt install live-build squashfs-tools live-boot xorriso isolinux netselect-apt -y
```

### Dosyaları oluşturma.

Öncelikle bu repoyu klonlayın.

```
git clone https://github.com/YmYLabs/AlfaWolf-Build.git
```

Klasörün içine girin.

```
cd AlfaWolf-Build
```

Klasörün içindekileri görmek için bunu girebilirsiniz

```
ls -la
```

### Builde başlama.

Şimdi bu komutu girin.

```
lb config
```

Bu gerekli dosyaları oluşturur.

Dağıtımımıza yüklenecek olan paketleri ayarlayalım.

```
sudo nano config/package-lists/live.list.chroot
```

Dosyaya bunları yapıştırın.

```bash
firmware-linux
live-boot
live-config
live-config-systemd
systemd-sysv
chromium
kde-standard
sddm
evolution
rhythmbox
vlc
shotwell
libreoffice
calamares
calamares-settings-debian
qt5-image-formats-plugins
qml-module-qtquick-controls
qml-module-qtquick-controls2
qml-module-qtquick-templates2
qml-module-qtquick-window2
qml-module-qtquick2
udisks2
dosfstools
e2fsprogs
btrfs-progs
f2fs-tools
xfsprogs
jfsutils
reiserfsprogs
ntfs-3g
grub-efi-amd64-bin
```