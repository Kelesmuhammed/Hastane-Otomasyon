# Hastane-Otomasyon

🏥 Kurumsal Hastane Otomasyon Sistemi (HBYS)

Bu proje; hastane içi idari, klinik ve hasta kabul süreçlerini dijital ortamda uçtan uca yönetmek amacıyla C# (.NET 8 / .NET 9), Windows Forms ve SQLite teknolojileri kullanılarak geliştirilmiş kapsamlı bir Hastane Bilgi Yönetim Sistemi (HBYS) masaüstü uygulamasıdır.


🎯 Projenin Amacı ve Kapsamı

Hastanelerdeki hasta kayıt, poliklinik/branş eşleştirme, çakışma kontrollü randevu oluşturma, e-reçete yazımı, laboratuvar tahlil takibi, tıbbi geçmiş (muayene) kayıtları, epikriz raporlama ve vezne/hizmet ücretlendirme işlemlerini Admin, Doktor ve Sekreter olmak üzere üç farklı yetki rolü altında güvenli ve hızlı bir şekilde yönetmektir.

⚙️ Teknik Özellikler ve Mimari
Taşınabilir Yerel Veritabanı (Zero-Config SQLite): Harici bir SQL Server kurulumuna gerek kalmadan, uygulama çalıştırıldığında App_Data/HastaneDB.db veritabanını, tabloları ve örnek verileri otomatik olarak oluşturur.
Güvenli Veri Katmanı (DAL): Tüm CRUD (Ekle, Listele, Güncelle, Sil) işlemleri merkezi DatabaseHelper sınıfı üzerinden %100 parametrik sorgularla (SQL Injection korumalı) yürütülür.
Modern Kurumsal Arayüz (UI/UX): Kurumsal renk paleti (#1e3d59), çift tamponlamalı (DoubleBuffered) modern tablolar ve TC Kimlik No (11 hane) / ücret girdi doğrulamaları (UIHelper) içerir.
Randevu Çakışma Kontrolü: Poliklinik -> Doktor -> Mesai Saati hiyerarşisiyle çalışır; aynı doktora veya aynı hastaya aynı tarih ve saatte mükerrer randevu verilmesini engeller.

🔐 Test Giriş Bilgileri
Admin: admin / admin123
Doktor: Ahmet / Ahmet123
Sekreter: Murat / karayel
