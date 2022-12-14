# 5ireChain-Node-Kurulum-Rehberi
![image](https://user-images.githubusercontent.com/101635385/207453430-865181a5-6d82-429f-8784-a265ac93b6d1.png)
<h1 align="center"> Selamlar,  5ireChain Testnet Kurulum rehberi by Hercules
</h1>



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



 ## 🟢 Github Giriş işlemi

* Öncelikle bir Github hesabına ihtiyacınız var ve özel token almanız gerekiyor. Adımlar aşağıdaki gibi.

* Settings Developer settings  Kısmına Giriyoruz
* Generate New Token ( Classic )  Tıklıyoruz 
* Açılan Sayfadan  workflow ve notifications  kısmını işaretliyoruz Ardından Genarate Token diyoruz
* Bize bir token verecek bunu kopyalayın bu şifreniz. 



![image](https://user-images.githubusercontent.com/101635385/207528783-e8e8b1bd-8161-49a0-be96-3d10f69384eb.png)


![image](https://user-images.githubusercontent.com/101635385/207528716-01fe8785-6070-4cec-b45f-ada8ba992d2c.png)





 ## 🟢 Kurulum
 
 Biraz önce aldığımız şifre ile giriş yapacağız
 
 ![image](https://user-images.githubusercontent.com/101635385/207529622-0b3cde55-aa33-4fb7-a3fc-a96f35bd4ccc.png)

* Username kısmına github kullanıcı adınız
* Şifre kısmına aldığınız token girip entera basın.
 
 
 
```shell
git clone https://github.com/5ire-tech/5ire-node-installer.git
```
![image](https://user-images.githubusercontent.com/101635385/207454867-937a7428-5098-49bf-b61e-28298f5a1d09.png)


```shell
cd 5ire-node-installer
```
![image](https://user-images.githubusercontent.com/101635385/207454912-1c875400-3d77-421f-9c69-b1d31122c008.png)


```shell
screen -S 5ire
```

```shell
chmod +x 5irechain-node-installer
```

```shell
./5irechain-node-installer
```
