
# Topantı Notları
Bu belgede yapılan toplantıların notları bulunacaktır. Her toplantı için tutulacak notlarda minimum beklenen bilgiler aşağıdaki gibidir:

* Tarih (YYYY-MM-DD formatında The ISO 8601 format)
* Katılımcılar
* Gündem
* Kararlar
* Bir sonraki aşamada yapılacaklar

## 2023-03-03

### Katılımcılar

* İsmail Can Dursun
* Murat Işık
* Volkan Özyılmaz

### Gündem

* Açık kaynak kodlu depreme uygun yazılım olup olmadığın konuşuldu.
* sahibinden.com sitesinde olduğu gibi harita üzerinden gösterim yapılabileceği gibi listeleme ile de gösterim yapılabilir.
* Routing: kapalı yolların da dahil edildiği bir routing sistemi gerekli.  
* Mapping için open street map kullanılabilir. Fakat tüm Türkiye tam olarak haritalanmamış.
  - Hangi harita sistemi tam olarak işimizi görür?
  - Google uydu imajları ile Microsoft uygu imajları giydirme için kullanılabilir.
* Gidilen yerlerin işaretlenmesi ve aynı yere başka ekiplerin gitmemesi sağlanabilir. Sistem otomatik olarak görev otomasyonu çıkarır ve ekipleri afet bölgelerinde müdahale edilecek yerlere atama için öneriler oluşturabilir. Operasyon yöneticisi bu önerileri kabul edip uygular veya uygulamaz.
* ARCGIS ticari bir ürün ve mapping için kullanılabilir. Dron gibi cihazlarla çekilen imajların gerekli eğip bükme işleri ile otomatikman hariyata giydirilmesi işi dahil bir çok modülü var.
  - https://enterprise.arcgis.com/en/cloud/latest/intro/enterprise-in-cloud.htm
  - https://learn.arcgis.com/en/projects/estimate-storage-capacity-with-drone-imagery/
* Sistemin offline çalışması gerekli. Ekiplerin her zaman internet erişimi olmuyor.

### Sonraki Aşamada Yapılacaklar

* Hangi harita sistemi tam olarak işimizi görür görevi Trello panosu üzerinde oluşturulacak (vozyilmaz)
* ARCGIS: AWS destekliyor. Serverless mi degil mi? Ne kadar ucreti var? 


## 2023-02-22

### Katılımcılar

* İsmail Can Dursun
* Murat Işık
* Volkan Özyılmaz

### Gündem

1. Karar almak için nasıl bir sistem izlenecek konusu konuşuldu. Detaylar community\_decision\_rules\_authorities dosyasından görülebilir. 
2. Yazılımın API ile anlaşma yapması, belki sadece backend'den oluşması konuşuldu. Farklı bir yaklaşım olarak sadece bir protokol olabileceği tartışıldı.
3. [QGIS](https://www.qgis.org/en/site/) haritalama modül olarak sisteme eklenebileceği tartışıldı. 
4. Gelen bir ihbarın nasıl teyitlenebileceği konuşuldu. 
  1. Avrupa birliğinin sunduğu uydu haritaları sistemi ile enkazların işaretlenebileceği (QGIS kullanılabilir) ve olmayan bir yere ihbar gelmesi durumunda bu bilgi ile aksiyon alınmasının sağlanabileceği konuşuldu. 
  2. İhbar geldikten sonra alanın kalabalık olmadığına bakılabileceği konuşuldu. 
5. Cep telefonları ile deprem anını anlayabilen bir mekanizma olduğu konuşuldu. Bu mekanizma ile depreme belli uzaklıktaki kişilere bildirim gönderilebilmesinin mümkünlüğü konuşuldu. 
6. Bina durumunu ultrasoniq bir yöntemle ölçebilen bir proje olduğu ve bu cihazların arama kurtarmacılara verilebileceği konuşuldu. 

### Kararlar

1. community\_decision\_rules\_authorities dosyasında belirtilen karar alma mekanizması kararları alındı. 

### Sonraki Aşamada Yapılacaklar
1. Karar alma belgesi oluşturulacak. (İsmail Can Dursun)
2. QGIS ile ilgili bilgi belgeleri oluşturulacak (Murat Işık)
3. Toplantı notlarının nerede duracağına karar verilecek
4. Afet Uygulamasi belgesindeki kullanıcı türleri kısmı güncellenecek (Volkan Özyılmaz)
5. Lojistik ile ilgili BlockDiagram dosyası incelenecek (Volkan Özyılmaz, Murat Işık)

