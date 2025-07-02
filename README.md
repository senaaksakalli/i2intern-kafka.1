# i2intern-kafka.1

Bu proje, i2i Systems staj programı kapsamında verilen  kafka konulu ödevin gerçekleştirilmesi amacıyla hazırlanmıştır.  
Amaç, **Apache Kafka’yı Docker kullanarak** bir konteyner ortamında çalıştırmak ve Kafka servislerinin sorunsuz şekilde ayağa kalktığını doğrulamaktır.  
Bu proje kapsamında Kafka'nın Zookeeper ile birlikte çalışır hale getirilmesi hedeflenmiştir.

## Kullanılan Komutlar ve Amaçları



### 1. `cd "C:\users\aksak\OneDrive\Masaüstü\kafka-proje"`
Bu komut ile Kafka projesinin yer aldığı klasöre geçiş yapılmıştır.  
Burada `docker-compose.yml` dosyası bulunmaktadır ve bu dosya, Kafka ve Zookeeper konteynerlerini tanımlar.



### 2. `docker-compose down`
Bu komut, önceden çalıştırılmış olan Kafka ve Zookeeper konteynerlerini durdurmak ve silmek için kullanılmıştır.  


### 3. `docker-compose up -d`
Bu komut ile `docker-compose.yml` dosyasındaki tanımlara göre Kafka ve Zookeeper konteynerleri yeniden başlatılmıştır.  
`-d` parametresi konteynerlerin arka planda (detached mode) çalışmasını sağlar.

Başlatılan servisler:
- `confluentinc/cp-zookeeper`
- `confluentinc/cp-kafka`


### 4. `docker ps`
Bu komut sayesinde çalışan tüm Docker konteynerleri listelenmiştir.  
Kafka ve Zookeeper servislerinin çalışıp çalışmadığı ve hangi portlar üzerinden erişildiği bu komutla doğrulanmıştır.


## 📷 Ekran Görüntüleri

> Kafka ve Zookeeper servislerinin başarıyla çalıştığına dair ekran görüntüleri eklenmiştir.


## NOT

Kafka’ya erişim, `localhost:9092` portu üzerinden yapılmıştır.


