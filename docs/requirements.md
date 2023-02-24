DEPREM UYGULAMASI (CASAD Computer Aided Support At Disasters) 

Amaç: Depremin hemen ardından yardım çağrılarının, ihtiyaçların, enkazların, kurtarma ve acil yardım ekiplerinin bulunduğu yerlerin, merkezi bir veri tabanında toplanarak, afete müdahale ekiplerinin planlama ve yönetim süreçlerine yardımcı olmaktır. (ismail Can Dursun)
SİSTEM HANGİ İHTİYAÇLARI CEVAPLAR? (Murat Işık)
Geliştirilecek sistem bugün afeti takip eden saatlerde ve günlerde yeterince efektif olarak cevaplanamayan aşağıdaki sorulara cevap üretecektir:
Sistemi yönetenlerin ilk aşamada / ilk günlerde merkezden analiz edip veri tabanına yükleyebileceği veriye ilişkin:
Afet tam olarak hangi yerleşim bölgelerini etkiledi?
Etkilenen nüfusun yaklaşık tahmini
Kaç bina etkilendi? Hangi binalar? Hangi adresler?
Ben afetten sağ veya yaralı olarak kurtuldum, yakınlarıma ulaşamıyorum. Onları nasıl bilgilendirebilirim?
Afet bölgesinde yakınım var, ulaşamıyorum, nasıl mesaj gönderebilirim?
Enkaz altında veya su baskınında mahsur kalan yakınım var, kurtarma ekiplerine nasıl bildirebilirim?
Kurtarma/müdahale ekibi mensubuyum. Hangi bölgeye, hangi binaya müdahale etmem en çok insana faydalı olur?
Hangi kurtarma ekibi hangi bölgede/hangi adreste çalışıyor?
Hangi bölgede/hangi adreste hangi uzmanlık alanlarına ihtiyaç var?
Hangi bölgede/hangi adreste hangi teknik ekipmana ihtiyaç var?
Hangi bölgeler müdahale edenler açısından riskler içeriyor?
Müdahale edilmemiş bölgeler/adresler hangileri?
Hangi bölgede, hangi yardım malzemelerine ihtiyaç var?
Tüm yakınlarını yitirmiş kimsesiz kalan, sahip çıkacak birilerine ihtiyaç duyan insanların listesi
Afetin ilerleyen günlerinde cevaplanacak sorular:
Kaç kişi yaralandı/öldü?
Yaralanan/ölen insanların kimlikleri


Uygulama farklı dilleri desteklemeli, farklı ülkeler için arayüz açılabilmelidir. Bu şekilde dünyanın herhangi bir ülkesindeki afet için o ülke insanları tarafından kullanılabilir olmalıdır. (ismail Can Dursun) (i18n/internationalization - vozyilmaz)

Uygulama içeriğinin belirlenmesinde mümkün olduğunca Arama Kurtarma Dernek ve ekiplerinden görüş alınır. Proje açık kaynak kodlu olarak github üzerinden yürütülmektedir:
https://github.com/ismailcandursun/CASAD
 (ismail Can Dursun)


KULLANICILAR (vözyılmaz)

Sistemi her vatandaş kullanabilir. Ancak bazı kuruluşlara daha fazla işlem yeteneği verilebilir.

En alt kullanıcı (1. seviye) sadece telefon numarası isim ve soyad bilgilerini girerek sisteme bilgi girişi yapar. Bu kişiler enkaz altında cep telefonu yanında olan ve kurtarılmayı bekleyenler, enkazdan kurtulmuş, ancak yakınları için yardım talebinde bulunanlar olabilir.

Bir üst seviyede (2. seviye) kullanıcı adı ve parola tanımlayan gönüllü sıradan vatandaşlar tanımlıdır. Bu kişilerin denetim ve görevleri daha sonra tanımlanacaktır.

3.seviyede onaylı gönüllüler bulunur. Bu kişiler daha önceden afetlerde gönüllü görev almış, veya afet sırasında AFAD, UMKE, AKUT, Belediye kurtarma ekipleri, Üniversite kulüpleri kurtarma ekipleri gibi kurumlardan onaylanmış kişilerdir. Bu kişiler  kurtarma ekipleri tanımlayabilecek, yeni enkaz alanları tanımlayabilecek, enkazlara kurtarma ekibi atayabilecek, yetkisi dahilindeki kurtarma ekipleri için teknik malzeme talebi açabilecek, ihtiyaç listesi girebilecektir.. Bu dernek veya ekiplerin logoları da uygulamada görünebilir.

4. seviyede 3. seviye kişileri tanımlayan, onaylayan, bunun dışında kendi ekipleriyle sahada olan, yukarıda sözü edilen dernek ve kuruluşlar bulunur.

5. Seviyedeki kullanıcılar başvuran 4. seviye dernekleri sistemde onaylayan kullanıcılardır.

6. Seviye kullanıcı 5. seviye kullanıcıları tanımlar.

7.Seviye kullanıcı Tüm sistem parametrelerini ayarlayan kullanıcılardır.
Afet bölgesine MAlzeme toplama alanlarından depremzedelere teslimat yapan kısa mesafe dağıtıcı kurye kullanıcılar
Yurdun çeşitli yerlerinden Afet Malzeme toplama alanlarına nakil yapan kurye kullanıcılar
(Kullanıcıları seviye seviye değil kavram olarak tanımlamak ve sistemdeki izinlerini tanımlamak doğrultusunda düşünmek taraftarıyım, böylece kullanıcıları aslında birer küme gibi görebiliriz ve kümeler birbirlerini kapsamak zorunda olmadıklarından kesişim kümeleri de bize kullanıcı tanımlatabilir. - vozyilmaz)



UYGULAMA MODÜLLERİ

Enkazlar (ismail Can Dursun)

Yıkılan binaların tespit edilerek GPS koordinatları ve mümkünse adresleri belirlenir. Afetin hemen ardından bölgeye gelen bir ekip dronlarla keşif yaparak yıkılan binaların koordinatlarını veritabanına girer. Diğer gönüllü arka plan ekipleri ise bu koordinatların adreslerini belirleyerek sisteme girer. 3. Seviye ve üstü kullanıcılar enkaz tanımı yapabilir. 4. Seviye ve üstü kullanıcılar hatalı girilen enkazları silebilir. Enkaz modülünde aşağıdaki maddeler göz önüne alınmalıdır.
Ekaz konumları
Enkaz hava ve yer fotoğrafları
Enkaz mimari planı (varsa, belki bir ekip belediyelerden bu girdileri sağlayabilir)
Enkazı inceleyen ekip veya uzmanların enkazla ilgili girdikleri bilgi ve uyarılar.
Enkaz durumları (Hafif hasarlı, Orta Hasarlı, Ağır hasarlı, çok ağır hasarlı.) Bu tanımlar ya yapılmalıdır.
Enkazdaki kurtarma ekipleri ve bulundukları sureler (dönüşümlü ekipler)
Enkaz civarında talep edilen ihtiyaç malzemeleri. (Yemek, su, giyecek, vs.)
Enkaz civarında sürekli bulunan vatandaşların listesi (yemek, su, tuvalet ihtiyaçlarının organize edilebilmesi için.)
Enkaz altında kaldığı düşünülen (aile veya yakınların bildirmesiyle) kişilerin bilgileri
Enkaz altından telefonla dışarıdan yardım isteyenler
Enkaz altında kaldığı Arama kurtarma ekibi tarafından teknolojik araçlarla tespit edilmiş, ancak henüz çıkarılmamış kişiler
Enkazdan sağ veya yaralı çıkarılanlar
Enkazdan çıkarılan cesetler




Kurtarma ekipleri (ismail Can Dursun)

Kurtarma ekipleri, ekip büyüklüğünü, özel yetenekleri, yanlarında bulundurdukları ekipman ve cihazları sisteme girerler. Ardından veri tabanından seçtiği, veya zaten bölgedeyse bulunduğu enkazda çalıştığını sisteme girer. Böylece diğer ekipler burada çalışma olduğunu görebilir. Kurtarma ekipleri diğer enkazdaki kurtarma ekiplerini görebilecek ve ekiplerin iletişim bilgilerine ulaşabilecektir. Kurtarma ekipleri vakit buldukça enkazdaki çalışma durumu, kurtarılan kişi sayısı, acil ihtiyaçlar, ekibe gerekli ekstra malzemeler, enkaz durumu, ses alındı mı, kaç kişi gibi bilgileri de sisteme gireceklerdir. Uygulamanın aşağıdaki maddeleri göz önünde bulundurması gerekmektedir.
Kurtarma Ekibi Tanımları
Kurtarma Ekibi Elemanları
Kurtarma Ekibinin yanındaki teknik malzemeler
Kurtarma Ekibinde eksik olan ve açil ihtiyaç duyulan teknik malzemeler
Kurtarma ekibinin yemek, su barınma vs gereksinimleri için ihtiyaç duyduğu malzemeler
Kurtarma ekibinin çalışma saatleri (dönüşümlü çalışan ekipler için)
Kurtarma Ekibinin enkazdan sağ veya yaralı çıkardığı kişiler
Kurtarma ekibinin enkazdan çıkardığı cesetler
Kurtarma ekibinin bulunduğu enkaz.
Kurtarma ekibi henüz herhangi bir enkaza atanmamışsa en son güncellediği konum.

Enkazdan çıkarılan yaralı ve çocuk kayıtları (ismail Can Dursun)

Enkazdan çıkarılan her yaralı bu enkaz kayıtlarına girilir. Sistemin verdiği numara çocuk veya yaralının yakasına iğnelenir.
 Yaralıların gönderildiği ambulans plakaları kişinin kaydına işlenir.Yaralıların ulaştıkları hastaneler veya yardım kuruluşları her yaralının yaka numarasını sisteme işler.

Enkazdan çıkarılan Cesetler (ismail Can Dursun)

Her ceset sisteme işlenir ve sistemin verdiği kod cesedin yakasına iğnelenir. Cesedin gönderildiği ambulans plakası sisteme işlenir. Ulaştığı morg sisteme işlenir. 
Defnedilmesi durumunda yaka numarasına defnedildiği mezarlık ve koordinatlar işlenir. Mümkünse (kimliği belirlenemeyenler için) yaka numarası gömüldüğü yere bir taş üzerine yazılır.

İhtiyaç malzemeleri (ismail Can Dursun)
Bu ihtiyaçlarda öncelikle kategoriler oluşturulmalıdır. Mesela barınma, ısınma, giyecek, yiyecek ve içecek, vs.
Yukarıda tanımlı belli seviyerlerdeki kullanıcılar ihtiyaçları sahadaki gönüllüler yardımıyla belirleyip giriş yapacaklardır. İhtiyaçları karşılamak isteyenler ise girilen ihtiyaçları gönderdikleri adreslere bu ihtiyaçların gönderildiği bilgisini girecekler. 
Afet bölgesinde x. Seviyedeki kullanıcılar, belirli ekiplerin (veya AFAD’ın) afet bölgesine yakın bölgelerde Gelen Malzeme Toplama Alanları belirleyip sisteme girmeliler.
Büyük şehirlerden Gelen Malzeme Toplama Alanlarına gelen malzemeler buradan gönüllü kuryeler aracılığıyla (Yaya, motosikletli, bisikletli, otomobil, vs) afet bölgesine dağıtılacaktır. Her kurye sistemde kullanıcı kurye olarak tanımlanacaktır. Uygulamanın bu modülü aşağıdaki maddeleri göz önünde bulunduracaktır:
Gelen Malzeme Toplama Alanı ile depremzedeler arasında çalışan gönüllü kuryeler. (yaya, bisikletli, motosiklet, otomobil, kamyonet)
Afet bölgesinde bulunmayan büyük şehirlerdeki yardımların toplanarak biriktirildiği Giden Malzeme Toplama Alanlarından, afet bölgesindeki toplama alanlarına nakil yapan kuryeler.
Afet bölgelerindeki gelen malzeme toplama alanları
Afet bölgesinde bulunmayan şehirlerdeki giden malzeme toplama alanları
Gelen Malzeme alanlarında görevli çalışan ve gönüllüler
Giden malzeme alanlarında görevli çalışan ve gönüllüler
Enkazlarda dağınık şekilde bulunan  ve malzeme dağıtımında görev alan gönüllüler
Gönüllü çalışanların vardiyalı ve dönüşümlü çalışacağı varsayılıp, bir zamanlama tablosunda görülmeleri, ve sistemin zamana göre kime erişilmesi gerektiğini göstermesi



Barınma  (ismail Can Dursun)
Barınma ihtiyacı olanlar sisteme yetişkin ve çocuk sayısı, yaşları, durumları (hafif yaralı, aile ferdi kayıpları, yaşları vs) girdikten sonra sistemde görünecektir. Ancak daha sonra bölgede yakınlarında olan bir 3. seviye kullanıcı bu kişileri görüp kendi onayını da girecektir. Barınma ihtiyacı olan kişi onaylanmamış da olsa sistemde görünecektir.

Evinde afetzede ağırlamak isteyenler, sistemdeki veriler yardımıyla bu kişilerle irtibata geçebilecek ve uygunluk sağlanması durumunda, sisteme bu kişilerin barınma ihtiyaçlarını sağlayabileceklerini gireceklerdir.

Barınma sağlayabilecek kişi ve kurumlar, doğrudan afetzedelerle irtibata geçmeden kendi barınma olanaklarını sisteme girebilecekler. Bu durumda yerleştirme işlemini daha yüksek seviyede bir kullanıcı yapacaktır.

Ulaşım (ismail Can Dursun)
Afetzedelerin buldukları barınma yerlerine ulaşmaları için bulundukları bölgeyi ve gidecekleri yerleri belirtebilecekler.
Afetzedelere gönüllü ulaşım sağlayan vatandaşlar ise araç bilgilerini ve kimlik bilgilerini girdikten sonra afetzedelerle doğrudan iletişim sağlayabileceklerdir. (18 yaş üstü için geçerli)




DİĞER ÖNERİLER:
—-------------------------------------------------------------
Avrupa birliği Acil Durum uydusundan yüksek çözünürlüklü haritaları alınarak Depremin ilk saatlerinden itibaren sisteme girilmesi. Bu konuda önceden oluşturulan ekipler depremin duyurulmasının hemen ardından, daha arama kurtarma ekipleri bölgeye ulaşmadan, uydu görüntülerini değerlendirerek sisteme enkaz girmeye başlayabilirler.
https://emergency.copernicus.eu/
Örnek harita: https://emergency.copernicus.eu/mapping/system/files/components/EMSR648_AOI02_GRA_MONIT01_r1_RTP01_v1.jpg
Cem Ayyıldız
—------------------------------------------------
Diğer işbirliği yapılabilecek organizasyonlar:
https://www.techtotherescue.org/earthquake-turkey-syria
Çağrı Tansuğ
—--------------------------------------------------

—-------------------------------------------------

Projeye Destek Verenler (Alfabetik)
(İsminizi alfabetik sıraya dikkat ederek aşağıdaki listeye ekleyebilirsiniz.)

Bunyad Dinç			bunyaddinc@gmail.com		Fotoğrafçı/Dağcı
Cem Ayyıldız 			cem.ayyildiz@gmail.com		Uzman/Mühendis
İsmail Can Dursun 		ismailcandursun@gmail.com		Mühendis/Dağcı
Murat Işık			murat.isik.istanbul@gmail.com	Mühendis/Dağcı
Mustafa Dağıstanlı 		dagmalp@gmail.com			Gazeteci
Volkan Özyılmaz		v@volkanozyilmaz.com		Uzman Yazılımcı/Mühendis
