# Ironfish Tutorial
Minimal Spesifikasi VPS

4Core vCPU 

6/8GB RAM

160GB/200GB SSD/NVME Storage

### Daftar dan Join Discord Ironfish

https://testnet.ironfish.network/signup

https://discord.gg/DQNsFwBtDQ

![image](https://user-images.githubusercontent.com/91402307/195981978-705f0141-8207-40f6-bdd6-c75fc59bd13d.png)

### Install Ironfish pilih No.1

``` 
wget -q -O ironfish.sh https://api.nodes.guru/ironfish.sh && chmod +x ironfish.sh && sudo /bin/bash ironfish.sh
```

![photo_2022-10-15_16-34-37](https://user-images.githubusercontent.com/91402307/195981562-794e3b9e-f9cd-462b-906b-9a4fe7837a05.jpg)

### Isi Nama Wallet, Nama Node sesuai dengan Nama Graffitin & isi Threads -1

<img width="263" alt="Screenshot_1" src="https://user-images.githubusercontent.com/91402307/195981793-de3bb6c0-4963-4630-89d2-9f5043d153e7.png">

### Masukkan ini dengan .
```
. $HOME/.bashrc
. $HOME/.bash_profile
```

### Masukkan ini dan akan terlihat nama node & Block Graffiti
```
cat $HOME/.ironfish/config.json
```

### Membuat Akun
```
ironfish accounts:create
```

### Isi tanda $ dengan graffiti
```
ironfish accounts:use $grafftimu
```

### Aktifkan Telemetry
```
ironfish config:set enableTelemetry true
```

### Check Status 
```
ironfish status -f
```

### Cek Reward/Poin setiap 12 jam akan mendapatkan 10 Point tulis Graffiti mu di Search

https://testnet.ironfish.network/leaderboard

![image](https://user-images.githubusercontent.com/91402307/195984483-dedea0b7-20ac-4e04-b019-c6e9a0633072.png)

## Cara Upgrade Versi Ironfish 
Pilih Nomor 2
```
wget -q -O ironfish.sh https://api.nodes.guru/ironfish.sh && chmod +x ironfish.sh && sudo /bin/bash ironfish.sh
```

## Backup Ironfish 
```
ironfish accounts:export
```
Backup dilakukan agar bisa berpindah pindah VPS Save semuanya di Notepad

## Cara Import  Ironfish
Ikuti tutorial Install Ironfish diatas hingga bagian (cat $HOME/.ironfish/config.json) setelah itu masukkann Command ini
```
ironfish accounts:import
```
Masukkan semua data yang sudah di backup di Notepad setelah itu Aktifkan Telemetry

# Command Berguna

### Stop Node
```
service ironfishd stop
```

### Start Node
```
service ironfishd start
```

### Cek Log Node
```
journalctl -u ironfishd -f
```

### Cek Log Miner
```
journalctl -u ironfishd-miner -f
```

### Migrasi
```
ironfish migrations:start -v
```

### Snapshot Block
Peringatan jika ingin mining Ironfish memerlukan VPS dengan Spek yang tinggi kalau bisa Support GPU jika tidak ada lebih baik tidak usah digunakan Command ini
```
apt install screen
screen -S ironfish
ironfish chain:download
```

Jika dalam proses download bisa Ctrl A+D untuk download di belakang untuk cara kembali ke Screen 
```
screen -r ironfish
```

 
