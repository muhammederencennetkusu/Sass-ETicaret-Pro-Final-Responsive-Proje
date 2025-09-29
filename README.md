# 🛒 Sass E-Ticaret Responsive Prototipi

Bu proje, modern bir e-ticaret sitesi için geliştirilmiş, ileri seviye **Sass** mimarisi ve **Responsive Tasarım** prensiplerini uygulayan bir frontend prototipidir. Ana odak noktası, temiz, sürdürülebilir CSS kodu üretmek ve mobil cihazlar için optimize edilmiş bir kullanıcı deneyimi (UX) sunmaktır.

## ✨ Temel Özellikler

* **Sass Mimarisi (7-1 Pattern):** Kod, `abstracts`, `components`, `layouts` gibi modüler klasörlere ayrılmıştır.
* **Tam Responsive Tasarım:** Header, Footer ve ürün listesi (Grid) tüm ekran boyutlarına (Mobil, Tablet, Desktop) dinamik olarak uyum sağlar.
* **Off-Canvas Menü:** Mobil cihazlar için profesyonel bir UX sağlayan, soldan açılır gizli navigasyon (Hamburger menü) yapısı JavaScript ile entegre edilmiştir.
* **Modern UI Bileşenleri:** Kartlar, butonlar, form girdileri ve etiketler (`on-sale`, `out-of-stock`) gibi standart e-ticaret bileşenleri tasarlanmıştır.

## 🛠️ Kullanılan Teknolojiler

* **Sass (SCSS):** CSS ön işlemcisi (Mixins, Variables, Nesting kullanılmıştır).
* **HTML5:** Semantik yapı.
* **CSS Grid & Flexbox:** Düzen (Layout) oluşturma.
* **JavaScript (Vanilla JS):** Off-Canvas menü etkileşimi için.
* **Font Awesome:** İkon kütüphanesi.

## 📁 Klasör Yapısı (Sass)
```bash
scss/
├── abstracts/        # Değişkenler, mixin'ler, fonksiyonlar
│   ├── _variables.scss
│   └── _mixins.scss
├── base/             # Temel HTML ve tipografi stilleri
├── components/       # Bağımsız ve yeniden kullanılabilir bileşenler
│   ├── _buttons.scss
│   ├── _forms.scss
│   └── _product-card.scss
├── layouts/          # Ana sayfa düzenleri
│   ├── _header.scss  # Off-canvas mantığı dahil
│   ├── _footer.scss
│   └── _product-listing.scss
├── pages/            # Sayfaya özel, büyük stiller (Opsiyonel)
└── style.scss        # Ana çıktı dosyası (Tüm parçaları import eder)

```

## 🚀 Başlangıç Kılavuzu

Bu projeyi yerel ortamınızda çalıştırmak için aşağıdaki adımları takip edin:

### 1. Sass Derleme (Compile)

Sass dosyalarını (`.scss`) tarayıcının okuyabileceği CSS dosyasına (`style.css`) dönüştürmek için terminalde projenin ana dizininde aşağıdaki komutu çalıştırın:

```bash
sass --watch scss/style.scss:css/style.css
