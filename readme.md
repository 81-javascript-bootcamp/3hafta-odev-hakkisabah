### Odev

- b ve m tuslarina basildiginda da ses calsin.
- satira tiklandiginda bgcolor ekleyelim.
- satira tiklandiginda soldaki imajda ilgili petin imajini gosterelim.


bonus
- birkac pet daha ekleyelim.

--- 

### Kişisel hesabımdaki kopya

https://github.com/hakkisabah/catanddog.space

###Neden
Projede özellik ve davranış geliştiriken amaç uygunluğu gözlemlenmiştir. 
Bu bağlamda küçük yaştaki çocukların kedi ve köpek seslerini eğlenceli ve iyi bir deneyimle öğrenmeleri için bir takım
kullanıcı deneyimini kolaylaştıran davranış ve eylemlerin amaca hizmet etmesi sağlanmıştır.

### Demo
https://www.catanddog.space/

####İstenilen davranışlara ek olarak :
- Sayfa ilk yüklenirken isim ve 2 adet pet apisinden verileri alır ve DOM'a aktarır
- Sayfa yüklendikten sonra hızlı yenileme için arka planda ikinci yükleme verilerini değişkene atar ve hazırda bekletir
- Her yenileme isteği sonrası bir sonraki yenileme için ilk baştaki işlemleri otomatik sağlar ve bu işlem her zaman asenkron çalışır
- b v m tuşlarına basıldığında ses çıkartır window.location.hash özelliği ile petin büyük resmine gider
- Ses için tıklandıktan sonra kullanıcıya büyük resmi görmek istediği sorulur. Eğer kullanıcı görmek istemezse büyük görsele hashleme yapılmaz
- Her büyük görsel görme isteğinde son tıklanılan butonun elementine "lastpoint" id attribute u atanır ve mantıksal sorgulamalar sonrası otomatikman kaldırılır
- Büyük resimdeki son tıklanan buton elementine gitme işlemini gerçekleştiren transparan buton tıklanırsa, son tıklanan elemente hasleme yapar ve ilgili element yanıp söner  
- Kullanıcı ilk dinlediği sesin büyük görsel sorusuna evet derse hemen ardından tekrar dinlemek istediğinde otomatikman büyük görsele gider
- Sayfa AWS CloudFront ve S3 servislerinde yardımı ile host edilmektedir ve Certificate Manager yardımı ile SSL üstünden yayım yapmaktadır
- Apilerden herhangi biri hata verirse bu otomatikman algılanır ve lokal görsel ve değişken değerleri kullanılır