# Goracle-Düğüm-Kurulumu

https://t.me/HerculesNode



Kaynak: https://teletype.in/@ttimmatti/goracle-node



**SİSTEM GEREKSİNİMLERİ**


Cpu: 1-2 cores

Ram: 4gb

Storage: 10gb SSD

Ubuntu: 20.04+

musluk: https://bank.testnet.algorand.network/




KURULUM


1. Goracle düğümünü başlatın:

```
sudo wget -qP /usr/bin/ https://staging.dev.goracle.io/downloads/latest-staging/goracle && sudo chmod u+x /usr/bin/goracle
```

![image](https://user-images.githubusercontent.com/119691371/228723108-5d3d9180-d406-4cac-b62f-0934092b5e97.png)


```
goracle init
```
![image](https://user-images.githubusercontent.com/119691371/228723140-20457426-5a2a-4958-8b45-c1d7dcc684a2.png)



1.1

İkisine de y deyin:

Continue? [y/N]?

Use Algonode Algorand API service (recommended)? [Y/n]?






1.2 
 Algonode API auth token girin ya da varsayılan olarak enter'a basın.
 
 
 
 
 
 
1.3
Ana algorand adresinizi girin (örneğin Pera wallet adresinizi. Myalgo wallet hacklenmiş o yüzden onu kullanmayın, zaten izin vermiyor)




1. https://testnet-app.goracle.io/nodes/optin adresine gidin.  Pera cüzdanınızla bağlanın (bağlanamıyorsanız ayarlardan tesneti seçin) ve ekran görüntüsünde belirtilen yerdeki adresinizi kopyalayın. 

![image](https://user-images.githubusercontent.com/119691371/228723166-961bce8e-5039-4578-bfb6-460583e92157.png)





2. Ve terminale yapıştırın.

![image](https://user-images.githubusercontent.com/119691371/228723178-ddcbb752-3bcc-4597-923d-46a9d7e47d5c.png)




3. Sonra enter'a basın.





1.4 Katılım adresinizi kaydetme:




1. terminalde çıkan katılım adresi kaydetme bağlantısını kopyalayıp tarayıcınızla açın.

![image](https://user-images.githubusercontent.com/119691371/228723198-52c062fe-dff5-482f-8c9d-1a19146ba9f4.png)





2. Sayfa şöyle görünmeli (yeniden Pera cüzdanınıza bağlanmanız gerekebilir):

![image](https://user-images.githubusercontent.com/119691371/228723215-de15af3f-14aa-42b5-8e38-22c3372c6d50.png)





3. Register butonuna basın. (yeşil buton).




4. Cüzdanınızdan işlemleri onaylayın. (Eğer Pera mobil ile yapıyorsanız mobil cüzdanınızı kontrol edin)
Eğer işlemleri onayladıktan sonra şu hatayı alıyorsanız lütfen açılır pencerelere onay verdiğinize ve test algonuz olduğuna emin olun. Yoksa musluktan alabilirsiniz.
https://bank.testnet.algorand.network/

![image](https://user-images.githubusercontent.com/119691371/228723243-501c2228-88c8-4942-b6c1-9dc6f7da4f35.png)





Ardından musluktan katılım adresinize test token yollayın. 
![image](https://user-images.githubusercontent.com/119691371/228723345-ef43cf17-00cb-4ad8-a0fd-e893b851a6d1.png)





Bir sonraki adımı sadece erişim kodu alanlar yapabilir. Eğer bu kodu almadıysanız bu adımı geçin. Halen düğümü kurup yayınları iletebilirsiniz ancak konsensüse katılamazsınız. Ayrıca yine de "Bir düğüm çalıştır" görevini tamamlamış olacaksınız.






1.5 Tokenları stake edin (Mail ile gönderilen kodu girin)



1. "Get Test Gora"ya tıklayın.

![image](https://user-images.githubusercontent.com/119691371/228723412-bc757605-56a0-4b85-bb2f-6740975c6076.png)





2. Mail'le aldığınız kodunuzu yapıştırın.

![image](https://user-images.githubusercontent.com/119691371/228723425-e72c8e58-80bd-42f6-850e-262f16682025.png)

![image](https://user-images.githubusercontent.com/119691371/228723462-3af14871-cf9e-4747-950f-987bad8ad8be.png)



3. Stake ekleyin.

![image](https://user-images.githubusercontent.com/119691371/228723476-c9564388-31e6-4ac9-9e27-a803ab788d42.png)

![image](https://user-images.githubusercontent.com/119691371/228723487-ae2810e2-9712-4d68-859e-2bd7fc0eda87.png)




Ardından cüzdanınızdan işlemleri onaylayın. Stake'inizin arttığını göreceksiniz.

![image](https://user-images.githubusercontent.com/119691371/228723503-f4a105c2-0196-48ec-9abc-5f05d666dc9f.png)




1.6 Son adım. Terminale dönün ve Enter'a basın.


------------------------------------------------------------




2. Docker yükleyin.

```
bash <(wget -qO- https://raw.githubusercontent.com/ttimmatti/dependencies/main/docker.sh)
```

![image](https://user-images.githubusercontent.com/119691371/228723535-dadb27d9-24a4-4557-af78-91b406745988.png)






3. Düğümü çalıştırın.

```
goracle docker-start --background
```

![image](https://user-images.githubusercontent.com/119691371/228723545-fa551bcb-0bcf-4dd8-8c4a-b3fe1f18a838.png)



4. Logları kontrol edin.

```
docker logs -f goracle-nr
```

Loglardan çıkmak için ctrl+c kısayolunu kullanın.

Kurulum tamamlandı:)
