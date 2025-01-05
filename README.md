# Giyim Mağazası Projesi

### Projenin Özeti:
Giyim mağazası projesi kapsamında, ilişkisel veritabanı tasarımı, mağaza yönetimi, müşteri ilişkileri, ürün yönetimi, sipariş işlemleri ve destek hattı gibi alanları kapsayacak şekilde hazırladık.

### Proje Amacı:
Projenin amacı, giyim mağazasının operasyonlarını daha etkin ve verimli bir şekilde yönetmektir. Bu veritabanı sistemi, müşteri, ürün, sipariş, mağaza, çalışan, şehir, fatura ve destek hattı gibi alanlardaki verileri düzenli bir şekilde yöneterek, mağaza operasyonlarının izlenmesini ve müşteri memnuniyetini artırmayı hedefler.

### Veri Modeli ve Tasarımı:
## 1.	Şehir Tablosu (Sehir)
     SehirID: Birincil anahtar.
     SehirAdi: Şehrin adı.
## 2.	Mağaza Tablosu (Magaza)
     MagazaID: Birincil anahtar.
     MagazaAdi: Mağaza adı.
     SehirID: Şehir tablosuna yabancı anahtar.
     Adres: Mağazanın adresi.
## 3.	Müşteri Tablosu (Musteri)
     MusteriID: Birincil anahtar.
     Ad, Soyad: Müşterinin adı ve soyadı.
     Eposta, Telefon: İletişim bilgileri.
     SehirID: Şehir tablosuna yabancı anahtar.
## 4.	Çalışan Tablosu (Calisan)
     CalisanID: Birincil anahtar.
     Ad, Soyad: Çalışanın adı ve soyadı.
     Eposta, Telefon: İletişim bilgileri.
     MagazaID: Mağaza tablosuna yabancı anahtar.
     Pozisyon: Çalışanın pozisyonu.
## 5.	Ürün Tablosu (Urun)
     UrunID: Birincil anahtar.
     UrunAdi: Ürün adı.
     Fiyat: Ürün fiyatı.
     Stok: Stok adedi.
## 6.	Sipariş Tablosu (Siparis)
     SiparisID: Birincil anahtar.
     MusteriID: Müşteri tablosuna yabancı anahtar.
     SiparisTarihi: Sipariş tarihi.
     ToplamTutar: Siparişin toplam tutarı.
## 7.	Sipariş Detayları Tablosu (SiparisDetaylari)
     SiparisDetayID: Birincil anahtar.
     SiparisID: Sipariş tablosuna yabancı anahtar.
     UrunID: Ürün tablosuna yabancı anahtar.
     Miktar, Fiyat: Sipariş detay bilgileri.
## 8.	Fatura Tablosu (Fatura)
     FaturaID: Birincil anahtar.
     SiparisID: Sipariş tablosuna yabancı anahtar.
     FaturaTarihi, ToplamTutar: Fatura bilgileri.
## 9.	Destek Hattı Tablosu (DestekHatti)
     DestekHattiID: Birincil anahtar.
     MusteriID: Müşteri tablosuna yabancı anahtar.
     SorunAciklamasi, SorunTarihi, Durum: Destek bilgileri.



### E-R Diyagramı

![WhatsApp Image 2024-12-30 at 12 07 20 PM](https://github.com/user-attachments/assets/fed91638-7016-4218-8d34-695a92a87d7d)
