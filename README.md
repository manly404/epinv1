<div align="center">

# epinv1

**Oyun hesabı, e-pin ve dijital ürün satışı için PHP tabanlı, yönetim panelli e-ticaret altyapısı**

![PHP](https://img.shields.io/badge/PHP-8-777BB4?logo=php&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-InnoDB-003545?logo=mariadb&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=black)
![Tasarım](https://img.shields.io/badge/Tasar%C4%B1m-Karanl%C4%B1k%20%26%20Mobil%20Uyumlu-3B82F6)

</div>

> Bu depo yalnızca tanıtım amaçlıdır, kaynak kod içermez. Ekran görüntülerindeki kullanıcılar ve siparişler örnek veridir.

![Ana sayfa](screenshots/01-home.jpg)

## Öne çıkanlar

- **Otomatik teslimat:** Satın alınan ürünün kodu anında hesaba teslim edilir.
- **Bakiye sistemi:** Shopier ile kartla ödeme, havale/EFT bildirimi ve kupon kodu.
- **Kampanyalar:** Süreli Fırsat Gecesi indirimleri, çekilişler, bonuslar, seviye ödülleri ve referans sistemi.
- **Tam yönetim paneli:** Mağazanın her parçası tek panelden yönetilir.
- **Mobil uyumlu:** Site ve panel; telefon, tablet ve masaüstüne uyum sağlar.

## Ekran görüntüleri

### Mağaza

| İlan Pazarı | Ürün Detayı |
|---|---|
| ![İlan Pazarı](screenshots/02-marketplace.jpg) | ![Ürün detayı](screenshots/03-product-detail.jpg) |
| **Giriş** | **Kayıt** |
| ![Giriş](screenshots/04-login.jpg) | ![Kayıt](screenshots/05-register.jpg) |

### Üye hesabı

| Siparişlerim | Bakiye Yükle |
|---|---|
| ![Siparişlerim](screenshots/06-orders.jpg) | ![Bakiye yükle](screenshots/07-add-balance.jpg) |
| **Çekilişler** | **Mobil görünüm** |
| ![Çekilişler](screenshots/08-giveaways.jpg) | <img src="screenshots/12-mobile-home.jpg" alt="Mobil ana sayfa" width="48%"> <img src="screenshots/13-mobile-orders.jpg" alt="Mobil siparişler" width="48%"> |

### Yönetim paneli

| Ana Sayfa | İstatistikler |
|---|---|
| ![Admin ana sayfa](screenshots/09-admin-dashboard.jpg) | ![İstatistikler](screenshots/10-admin-analytics.jpg) |
| **Ürünler** | |
| ![Ürünler](screenshots/11-admin-products.jpg) | |

## Özellikler

**Mağaza ve üyelik**

- Kategori, ilan pazarı, ürün arama ve filtreleme
- Siparişler, bildirimler, destek talepleri ve giriş geçmişi
- Duyurular ve yorumlar
- Sözleşme ve yasal sayfalar

**Yönetim paneli**

- Satış grafikleri, istatistikler ve "ilgilenmen gerekenler" listesi
- Ürün, stok, kategori, sipariş ve üye yönetimi
- Çekiliş, kupon, bonus, seviye ödülü, referans ve Fırsat Gecesi yönetimi
- Canlı kullanıcı takibi, giriş kayıtları, destek talepleri ve toplu bildirim
- Site ayarları, sayfa yönetimi, slider, banka bilgileri ve bakım modu

## Güvenlik

| Alan | Önlem |
|---|---|
| **SQL enjeksiyonu** | Kullanıcı girdileri parametreli sorgularla (PDO) işlenir |
| **XSS** | Çıktılar kaçışlanır, bildirim bağlantıları doğrulanır |
| **Şifreler** | Tek yönlü `password_hash` ile saklanır |
| **Oturum** | `HttpOnly`, `Secure` ve `SameSite` çerezleri; girişte oturum kimliği yenilenir |
| **Kaba kuvvet** | Veritabanı tabanlı giriş denemesi sınırı; kayıtta sunucuda üretilen görsel captcha |
| **CSRF** | Yönetim panelindeki tüm işlemlerde token doğrulaması |
| **Yetkilendirme** | Panel ve hesap sayfalarında sunucu tarafında rol ve sahiplik kontrolü |
| **Para işlemleri** | Satın alma ve çekiliş ödemeleri satır kilitli işlemlerle yürütülür, eşzamanlı isteklerde çift harcama engellenir |
| **Ödeme** | Shopier bildirimleri HMAC imzasıyla doğrulanır |
| **Dosya yükleme** | Uzantı ve içerik kontrolü; yükleme klasöründe betik çalıştırma kapalıdır |
| **Gizli bilgiler** | Anahtarlar `.env` dosyasında tutulur, bu dosya web'den erişilemez |

## Teknolojiler

PHP 8 · MariaDB (PDO) · Apache · HTML, CSS, JavaScript · Chart.js · Quill · DataTables · Shopier

## Satın alma

Satın almak veya bilgi almak için [GitHub profilimdeki](https://github.com/manly404) Telegram adresinden bana ulaşabilirsiniz.
