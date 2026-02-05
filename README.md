# 🛒 NovaStore E-Ticaret Veri Yönetim Sistemi

[cite_start]Bu proje, bir e-ticaret sitesinin veri tabanı mimarisini tasarlamak, ilişkisel tablolar oluşturmak ve işletme yönetimi için gerekli veri analizlerini SQL sorguları ile gerçekleştirmek amacıyla geliştirilmiştir. [cite: 362, 364]

## 📋 Proje Özeti
Yeni kurulan **NovaStore** adlı e-ticaret platformu için; [cite_start]ürünlerin, müşterilerin ve siparişlerin yönetileceği kapsamlı bir SQL Server veri tabanı iskeleti kurulmuş ve senaryo gereği raporlamalar yapılmıştır. [cite: 366, 367]

## 🛠️ Teknik Gereksinimler & Yapı
Proje süresince aşağıdaki SQL kavramları ve teknikleri aktif olarak kullanılmıştır:
- [cite_start]**DDL (Data Definition Language):** Veri tabanı ve tablo yapılarının oluşturulması (PK, FK, Identity, Unique, Default kısıtlamaları). [cite: 368, 369]
- [cite_start]**DML (Data Manipulation Language):** Test verilerinin (Dummy Data) sisteme dahil edilmesi. [cite: 400, 401]
- [cite_start]**DQL (Data Query Language):** Karmaşık Join işlemleri, Gruplama (Group By), Zaman Analizleri (DATEDIFF). [cite: 407, 408]
- [cite_start]**İleri Seviye Nesneler:** Kolay raporlama için `View` oluşturma ve Veri tabanı `Backup` alma işlemleri. [cite: 428, 429, 432]

## 🗂️ Veri Tabanı Şeması
[cite_start]Veri tabanı aşağıdaki 5 ana tablo üzerine kurgulanmıştır: [cite: 374]
1. [cite_start]**Categories:** Ürün kategorilerini tutar. [cite: 375]
2. [cite_start]**Customers:** Müşteri bilgilerini ve iletişim verilerini saklar. [cite: 385]
3. [cite_start]**Products:** Ürün detaylarını ve stok bilgilerini barındırır. [cite: 379]
4. [cite_start]**Orders:** Müşterilerin verdiği siparişlerin genel bilgilerini içerir. [cite: 390]
5. [cite_start]**OrderDetails:** Siparişler ve ürünler arasındaki ilişkiyi kuran ara tablodur. [cite: 395]



## 🚀 Raporlama ve Analiz Örnekleri
Proje kapsamında aşağıdaki iş sorularına yanıt veren SQL raporları hazırlanmıştır:
- [cite_start]**Stok Takibi:** Kritik stok seviyesindeki (20'den az) ürünlerin listelenmesi. [cite: 410]
- [cite_start]**Müşteri Sipariş Geçmişi:** Müşteri bazlı sipariş tarihleri ve toplam tutarların Join ile birleştirilmesi. [cite: 413]
- [cite_start]**Ciro Analizi:** Şirkete en çok kazanç sağlayan müşterilerin belirlenmesi (SUM & Group By). [cite: 422]
- [cite_start]**Zaman Analizi:** Siparişlerin üzerinden geçen gün sayısının hesaplanması. [cite: 425]

## 📂 Dosya İçeriği
- [cite_start]`AdSoyad_NovaStore_Proje.sql`: Tüm SQL kodlarını (Tablo oluşturma, veri girişi ve sorgular) içeren ana dosya. [cite: 437, 439]

## ⚙️ Kurulum
1. SQL Server Management Studio (SSMS) uygulamasını açın.
2. `.sql` dosyasındaki kodları bir query penceresine kopyalayın.
3. Önce veri tabanı oluşturma kısmını, ardından tablo ve veri girişi kısımlarını sırasıyla çalıştırın.
4. [cite_start]Yedekleme (Backup) komutu için `C:\Yedek` klasörünün bilgisayarınızda mevcut olduğundan emin olun. [cite: 433]

---
[cite_start]*Bu çalışma, TNCGROUP bünyesindeki staj programı kapsamında hazırlanmıştır.* [cite: 15]
