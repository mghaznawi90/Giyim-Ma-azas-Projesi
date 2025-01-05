# Giyim Mağazası Projesi

### Projenin Özeti:
Giyim mağazası projesi kapsamında, ilişkisel veritabanı tasarımı, mağaza yönetimi, müşteri ilişkileri, ürün yönetimi, sipariş işlemleri ve destek hattı gibi alanları kapsayacak şekilde hazırladık.

### Proje Amacı:
Projenin amacı, giyim mağazasının operasyonlarını daha etkin ve verimli bir şekilde yönetmektir. Bu veritabanı sistemi, müşteri, ürün, sipariş, mağaza, çalışan, şehir, fatura ve destek hattı gibi alanlardaki verileri düzenli bir şekilde yöneterek, mağaza operasyonlarının izlenmesini ve müşteri memnuniyetini artırmayı hedefler.

### Veri Modeli ve Tasarımı:
1.	Şehir Tablosu (Sehir)
o	SehirID: Birincil anahtar.
o	SehirAdi: Şehrin adı.
2.	Mağaza Tablosu (Magaza)
o	MagazaID: Birincil anahtar.
o	MagazaAdi: Mağaza adı.
o	SehirID: Şehir tablosuna yabancı anahtar.
o	Adres: Mağazanın adresi.
3.	Müşteri Tablosu (Musteri)
o	MusteriID: Birincil anahtar.
o	Ad, Soyad: Müşterinin adı ve soyadı.
o	Eposta, Telefon: İletişim bilgileri.
o	SehirID: Şehir tablosuna yabancı anahtar.
4.	Çalışan Tablosu (Calisan)
o	CalisanID: Birincil anahtar.
o	Ad, Soyad: Çalışanın adı ve soyadı.
o	Eposta, Telefon: İletişim bilgileri.
o	MagazaID: Mağaza tablosuna yabancı anahtar.
o	Pozisyon: Çalışanın pozisyonu.
5.	Ürün Tablosu (Urun)
o	UrunID: Birincil anahtar.
o	UrunAdi: Ürün adı.
o	Fiyat: Ürün fiyatı.
o	Stok: Stok adedi.
6.	Sipariş Tablosu (Siparis)
o	SiparisID: Birincil anahtar.
o	MusteriID: Müşteri tablosuna yabancı anahtar.
o	SiparisTarihi: Sipariş tarihi.
o	ToplamTutar: Siparişin toplam tutarı.
7.	Sipariş Detayları Tablosu (SiparisDetaylari)
o	SiparisDetayID: Birincil anahtar.
o	SiparisID: Sipariş tablosuna yabancı anahtar.
o	UrunID: Ürün tablosuna yabancı anahtar.
o	Miktar, Fiyat: Sipariş detay bilgileri.
8.	Fatura Tablosu (Fatura)
o	FaturaID: Birincil anahtar.
o	SiparisID: Sipariş tablosuna yabancı anahtar.
o	FaturaTarihi, ToplamTutar: Fatura bilgileri.
9.	Destek Hattı Tablosu (DestekHatti)
o	DestekHattiID: Birincil anahtar.
o	MusteriID: Müşteri tablosuna yabancı anahtar.
o	SorunAciklamasi, SorunTarihi, Durum: Destek bilgileri.





![WhatsApp Image 2024-12-30 at 12 07 20 PM](https://github.com/user-attachments/assets/fed91638-7016-4218-8d34-695a92a87d7d)
