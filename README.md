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







<br><br><br><br><br><br>

 ## 🟢 Şimdilik Aşağıdaki Kodlar Kullanılmıyor....
 <br>
 ## 🟢 Github Giriş işlemi

* Öncelikle bir Github hesabına ihtiyacınız var ve özel token almanız gerekiyor. Adımlar aşağıdaki gibi.

* Settings Developer settings  Kısmına Giriyoruz
* Generate New Token ( Classic )  Tıklıyoruz 
* Açılan Sayfadan  workflow ve notifications  kısmını işaretliyoruz Ardından Genarate Token diyoruz
* Bize bir token verecek bunu kopyalayın bu şifreniz. 



![image](https://user-images.githubusercontent.com/101635385/207528783-e8e8b1bd-8161-49a0-be96-3d10f69384eb.png)


![image](https://user-images.githubusercontent.com/101635385/207528716-01fe8785-6070-4cec-b45f-ada8ba992d2c.png)





 ## 🟢 - 1 -
 
 Biraz önce aldığımız şifre ile giriş yapacağız
 
 ![image](https://user-images.githubusercontent.com/101635385/207529622-0b3cde55-aa33-4fb7-a3fc-a96f35bd4ccc.png)

* Username kısmına github kullanıcı adınız
* Şifre kısmına aldığınız token girip entera basın.
 
 
 
```shell
git clone https://github.com/5ire-tech/5ire-node-installer.git
```


 ## 🟢 - 2 -


Şimdi, '5ire-node-installer' adlı bir klasör görebilirsiniz, o klasöre gidin ve 5irechain-node-installer adlı bir dosya var.
<br>
Aşağıdaki komutu çalıştırarak dizine gidin:

```shell
cd 5ire-node-installer
```
![image](https://user-images.githubusercontent.com/101635385/207454912-1c875400-3d77-421f-9c69-b1d31122c008.png)


<br>
Screen oluşturalım

```shell
screen -S 5ire
```

 ## 🟢 - 3 -
 
 <br>
izinleri verelim


```shell
chmod +x 5irechain-node-installer
```

 ## 🟢 - 4 -
 
 <br>
Kurulumu başlatalım

```shell
./5irechain-node-installer
```

 ## 🟢 - 5 -
 
 <br>
Kurulum başladı

![image](https://user-images.githubusercontent.com/101635385/207533112-f6c401f8-9ef2-4636-8cde-ea56aa6277fe.png)

 ## 🟢 - 6 -
 
 <br>
Terminal isim soracaktır Node isminizi Giriniz

![image](https://user-images.githubusercontent.com/101635385/207533241-921f2f9b-2694-458a-bacc-9cf82bdad102.png)

 ## 🟢 - 7 -
 
 <br>
Senkronize işlemleri başladı ve biraz uzun sürebilir.

![image](https://user-images.githubusercontent.com/101635385/207533321-1384e2bf-d1b3-4c0e-a145-f0502ab3b1b3.png)


 ## Kurulum şimdilik Bu kadar
 


