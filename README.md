# 🛒 NovaStore E-Ticaret Veri Yönetim Sistemi

Bu proje, bir e-ticaret sitesinin veri tabanı mimarisini tasarlamak, ilişkisel tablolar oluşturmak ve işletme yönetimi için gerekli veri analizlerini SQL sorguları ile gerçekleştirmek amacıyla geliştirilmiştir.

## 📋 Proje Özeti
Yeni kurulan **NovaStore** adlı e-ticaret platformu için; ürünlerin, müşterilerin ve siparişlerin yönetileceği kapsamlı bir SQL Server veri tabanı iskeleti kurulmuş ve senaryo gereği raporlamalar yapılmıştır.

## 🛠️ Teknik Gereksinimler & Yapı
Proje süresince aşağıdaki SQL kavramları ve teknikleri aktif olarak kullanılmıştır:
- **DDL (Data Definition Language):** Veri tabanı ve tablo yapılarının oluşturulması (PK, FK, Identity, Unique, Default kısıtlamaları).
- **DML (Data Manipulation Language):** Test verilerinin (Dummy Data) sisteme dahil edilmesi.
- **DQL (Data Query Language):** Karmaşık Join işlemleri, Gruplama (Group By), Zaman Analizleri (DATEDIFF).
- **İleri Seviye Nesneler:** Kolay raporlama için `View` oluşturma ve Veri tabanı `Backup` alma işlemleri.

## 🗂️ Veri Tabanı Şeması
Veri tabanı aşağıdaki 5 ana tablo üzerine kurgulanmıştır:
1. **Categories:** Ürün kategorilerini tutar.
2. **Customers:** Müşteri bilgilerini ve iletişim verilerini saklar.
3. **Products:** Ürün detaylarını ve stok bilgilerini barındırır.
4. **Orders:** Müşterilerin verdiği siparişlerin genel bilgilerini içerir.
5. **OrderDetails:** Siparişler ve ürünler arasındaki ilişkiyi kuran ara tablodur.

## 🚀 Raporlama ve Analiz Örnekleri
Proje kapsamında aşağıdaki iş sorularına yanıt veren SQL raporları hazırlanmıştır:
- **Stok Takibi:** Kritik stok seviyesindeki (20'den az) ürünlerin listelenmesi.
- **Müşteri Sipariş Geçmişi:** Müşteri bazlı sipariş tarihleri ve toplam tutarların Join ile birleştirilmesi.
- **Ciro Analizi:** Şirkete en çok kazanç sağlayan müşterilerin belirlenmesi (SUM & Group By).
- **Zaman Analizi:** Siparişlerin üzerinden geçen gün sayısının hesaplanması.

## 📂 Dosya İçeriği
- `NovaStore_Proje.sql`: Tüm SQL kodlarını (Tablo oluşturma, veri girişi ve sorgular) içeren ana dosya.

## ⚙️ Kurulum
1. SQL Server Management Studio (SSMS) uygulamasını açın.
2. `.sql` dosyasındaki kodları bir query penceresine kopyalayın.
3. Önce veri tabanı oluşturma kısmını, ardından tablo ve veri girişi kısımlarını sırasıyla çalıştırın.
4. Yedekleme (Backup) komutu için `C:\Yedek` klasörünün bilgisayarınızda mevcut olduğundan emin olun.
