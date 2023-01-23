# 5ireChain-Node-Kurulum-Rehberi
![image](https://user-images.githubusercontent.com/101635385/207453430-865181a5-6d82-429f-8784-a265ac93b6d1.png)
<h1 align="center"> Selamlar,  5ireChain Testnet Kurulum rehberi by Hercules
</h1>

<h1 align="center"> Bu Rehber 5ire Tarafından Mail alan Seçilen Kişiler içindir. Seçilmediyseniz Kurulum Yapmayınız.

## 🟢 Linkler:

 * [Yeni Node Testnet Telegram Kanalı](https://t.me/HerculesNode)
 * [5ireTelegram Destek Kanalı](https://t.me/x5hirechain)
 * [Twitter](https://twitter.com/Hercules4413)

## 🟢 Sistem Gereksinimleri

#Minimum Gereksinimler

* İşlemci :
* Çekirdek: 4
* Bellek : 8 GB
* Depolama : 100GB SSD


#Önerilen Gereksinimler

* İşlemci :
* Çekirdek: 8
* Bellek : 32GB
* Depolama : 100GB SSD
<br><br><br><br>

 ## 🟢 - Aşağıdaki komutu kullanarak Docker görüntüsünü indirin -
 
```shell
docker pull 5irechain/5ire-thunder-node:0.10
```
 
```shell
screen -S 5ire
``` 

<br><br><br>

 ## 🟢 - Full Node Kurmak için Bu kodu kullanın 
 
 * Tam bir düğüm için aşağıdaki komutu çalıştırın

<br>  
 Burada Sadce kodda bulunan -name NODE-İSMİNİZ  Bu kısma kendi isminizi yazacaksınız
 
```shell
docker run -p 30333:30333 -p 9933:9933 -p 9944:9944 5irechain/5ire-thunder-node:0.10 --port 30333  --ws-external --ws-port 9944 --rpc-external --rpc-port 9933 --rpc-cors all --no-telemetry --name NODE-İSMİNİZ --bootnodes /ip4/3.19.122.7/tcp/30333/p2p/12D3KooWNLQPtTkKwapACfMas7vyM4gujwnevxfgXUyTGno3bDpY --pruning archive
```
 <br><br><br>
 
 ## 🟢 - Doğrulayıcı Node Kurmak için Bu kodu kullanın 
 
 * Doğrulayıcı düğüm için aşağıdaki komutu çalıştırın:
 
 <br>  Burada Sadce kodda bulunan -name NODE-İSMİNİZ  Bu kısma kendi isminizi yazacaksınız
 
```shell
docker run -p 30333:30333 5irechain/5ire-thunder-node:0.10 --port 30333 --no-telemetry --name NODE-İSMİNİZ --bootnodes /ip4/3.19.122.7/tcp/30333/p2p/12D3KooWNLQPtTkKwapACfMas7vyM4gujwnevxfgXUyTGno3bDpY --pruning archive --validator
```
<br>
<br>
 
 ![image](https://user-images.githubusercontent.com/101635385/208252070-92865318-c996-4013-9e7b-2217ccc8369d.png)
 
 <br>


![image](https://user-images.githubusercontent.com/101635385/208251835-12619bbf-e55f-4ae8-ab02-d5774d95c668.png)









 ## Kurulum şimdilik Bu kadar
 


