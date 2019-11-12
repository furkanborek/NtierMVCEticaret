# NtierMVCEticaret
YMS3132 Öğrencileri Tarafından Geliştirilmekte Olan bir E-Ticaret Sitesi Projesidir.

E Ticaret Sitesi Dokümantasyon

Proje Açıklaması
E-Ticaret sitesi olarak yazılan bu proje de kullanıcı sitede istediği kategorideki ürünler arasında dolaşabilir ve ürünlerde filtreleme yapabilir. Kullanıcı istediği ürünü sepetine atabilir ve istediğinde sepetinde hangi ürünlerin bulunduğunu ve toplam olarak ne kadar ödemesi gerektiğini görebilir. Satın alma işlemini yapmak istediğinde kart bilgilerini ve adresini girerek satın alma işlemini tamamlar.
Projenin Teknik Bilgileri

	Ntier ve MVC Mimari
	Code First EAV modeli Veri Tabanı
	Mail Gönderme, Fotoğraf Yükleme ve Şifreleme Sınıfları
	Web Api Kullanımı:
1)	Kargo Api
2)	Loglama Api
3)	Fake Data Api
	Önyüz tasarımında Kullanılanlar:
1)	Javascript
2)	Ajax
	Admin Özel Sayfa (Urun ekleme vb. için)
	Member için sayfalar

Master’ın Görevleri

	Proje Başlangıcında Projenin Mimarisini oluşturmak, gerekli sınıfları projeye entegre etmek ve referansları vermek
	Projenin yapılış zamanı sürecinde proje çalışanlarının yaptıkları işlemlerde onları gözlemlemek ve çıkan sorunlarda eğer takım arkadaşı o sorunu çözemiyorsa sorunun çözümünü devir alarak sorunu çözmek
	Takım arkadaşlarının psikolojik durumlarını göz önünde bulundurmak ve takım arkadaşlarına destekçi olmak
	Proje çalışanı kendi üzerine düşen görevi tamamladıktan sonra commit ve push işlemlerinden önce güncel projede çalıştığının teyidini almak ve projenin güncel versiyonunda çalıştığının onayını altıktan sonra commit etmesi sonucunda Master olarak projeyi o kişiden çekerek Master’i güncel tutmak.

Önemli Bilgi: Proje deki göreve başlarken master’ın söylediği zamanda başlamaya dikkat edilmelidir. Master’in sizin proje üzerinde çalıştığınızdan haberi olmalıdır. Önemli işlemleri (commit vb.) işlemler yapılırken master’a bilgi verilmeli ve onay beklenmelidir. Projeye başlarken projenin güncel halini master’dan çektiğinize emin olmalısınız.

Görev Dağılımı

	Furkan BÖREK (Master)
1)	Ntier ve MVC mimarisinin kurulması
2)	Gerekli Framework’lerin indirilmesi
3)	Katmanlar arasında referansların verilmesi
4)	Web. Config’e bağlantı yazısının verilmesi
5)	Mail Gönderme, Fotoğraf Yükleme, Şifreleme Sınıflarının Yapılması
6)	Web sitesi görsellerinin MVCUI katmanında mevcut hale getirilmesi
7)	Katmanlardaki gerekli klasörlerin açılması (Design Patterns vb.)

	Esra SANCAK
1)	Veri tabanın Code First yazılması
2)	Veri tabanına EAV modelinin entegrasyonu
3)	Ürün ile Kategori arasında ilişkinin çoka çok olarak yapılması
4)	Veritabanı sınıflarının MAP katmanında düzenlenmesi(AppuserMap vb.)
5)	DAL katmanında MyContext sınıfının oluşturulup Veritabanı işlemlerini sonlandırmak. Connection name =”MyConnection”
6)	Strategy patterni
7)	BLL katmanında Repository’lerin oluşturulması
	Tarık 
1)	İlk olarak Kargo Firmasının Web Api’si yazılacak
2)	Backend kodları yazılacak(Enes ile ortak çalışarak)
	ENES
1)	İlk olarak Loglama Api’si yazılacak
2)	Ek veritabanı
3)	Backend kodları yazılacak(Tarık ile ortak çalışarak)
	CEM
1)	Frontend Kodları yazılacak ve Gökhan ile birlikte ortaklaşa çalışacaklar.
	GÖKHAN
1)	Frontend Kodları yazılacak ve Cem ile birlikte ortaklaşa çalışacaklar.
	OZAN
1)	Api Entegrasyonu E Ticaret
	Alp
1)	Proje master’a gelmeden önce detaylı test işleminden geçecek.







Yapılanlar
	Master
1)	Bogus Dal katmanına yüklendi
2)	EntityFramework 6.2.0 BLL, COMMON, DAL, MAP, MVCUI katmanlarına yüklendi
3)	Microsoft. AspNet. WebApi. Client 5.2.7 MVCUI katmanına yüklendi
4)	BLL katmanı COMMON, DAL, MODEL katmanında referans aldı
5)	DAL katmanı MAP ve MODEL katmanında referans aldı
6)	MAP katmanı MODEL katmanından referans aldı
7)	MVCUI katmanı BLL, COMMON ve MODEL katmanında referans aldı.
8)	MVCUI katmanının Web. Config’e Connection String yazıldı name "MyConnection" olarak verildi.
9)	COMMON katmanına Mail gönderme, Fotoğraf yükleme, Şifreleme Sınıfları eklendi
10)	MVC FlatAdmin Eklendi

Zaman Yönetimi
1)	Tarık => 4 gün  (Api entegrasyonu Kargo)------- 14 de basla
2)	Ozan => (Api Entegrasyonu E Ticaret) -------- 14 de basla
3)	Esra => 4 gün (veri tabanı) ------ 14 de basla
4)	Enes => 4 gün (Loglama ve ek veri tabanı) ----- 14 basla 
5)  Kasım 18 Tarık (Api),Enes(Loglama) ve Esra veritabanı bitiyor... -- Yetişir...
6)  Aralık 5 Tarık ve Enes Backend bitişi...
7)  Aralık 10 Cem ve Gökhan Frontend bitişi...
8)  Aralık 13 Ozan Api Entegrasyon Bitişi...
9) 	2020 Ocak 3 Emre Alp Test bitişi
10) 2020 Mart 3 Proje Live'a acılısı...
