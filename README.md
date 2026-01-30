# AlfaWolf Linux Build Repository.

## Nasıl yapılır?

### Gerekli uygulamaları yükleme.
sudo apt update && sudo apt upgrade -y
sudo apt install live-build squashfs-tools live-boot xorriso isolinux netselect-apt -y

### Dosyaları oluşturma.
Öncelikle buildi yapacağımız klasörü oluşturalım.
mkdir -p AlfaWolf
Sonra dosyanın içine girelim.
cd AlfaWolf
Şimdi bu repoyu klonlayın.
