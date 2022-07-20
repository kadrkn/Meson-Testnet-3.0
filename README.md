# Meson-Testnet-3.0
Meson Network Testnet 3.0 Kurulum Rehberi

Sistem Gereksinimleri; 2 CPU - 2 GB RAM - 20 GB SSD

https://dashboard.meson.network/register buradan üyelik oluşturuyoruz.

Önce " sudo apt-get update -y && sudo apt-get install wget -y " komutu ile sunucuyu güncelleyelim.

" sudo ufw allow 443 " komutu ile 443 numaralı portu açalım !

Kayıt olduğumuz sitedei "Nodes" kısmına girelim ve burada 1. download & install kısmındaki " wget 'https://staticassets.meson.network/public/meson_cdn/v3.1.18/meson_cdn-linux-amd64.tar.gz' && tar -zxf meson_cdn-linux-amd64.tar.gz && rm -f meson_cdn-linux-amd64.tar.gz && cd ./meson_cdn-linux-amd64 && sudo ./service install meson_cdn " komuutu girelim.

Daha sonrasında set token and config kısmındaki " sudo ./meson_cdn config set --token=ydckgkfwrazvnyoznmrvktdl --https_port=443 --cache.size=30 " komutu ile token adını oluşturalım. Ben olduğu gibi kopyala yapştırdım. 

" sudo ./service start meson_cdn " komutu ile servisimizi çalıştıralım.

Daha sonrasnda https://dashboard.meson.network/user_node sayfasındaki Manager Nodes kısmında node görünecektir. " sudo ./service status meson_cdn " komutu ile de sunucumuzda node durumunu görebiliriz.
