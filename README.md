# Sass-Modular-Kit

## Modüler ve Responsif Ön Yüz Başlangıç Kiti

Bu proje, modern web projeleri için tasarlanmış, tamamen modüler (parçalara ayrılmış) ve ölçeklenebilir bir CSS mimarisinin canlı örneğidir. Tüm stiller **Sass (SCSS)** ile yazılmıştır ve endüstri standardı olan **7-1 Pattern** metodolojisini takip eder.

Bu kit, bir projenin büyümesi sırasında kod karmaşasını önlerken, geliştiricilere hız ve sürdürülebilirlik sağlamak için tasarlanmıştır.

---

## 🚀 Temel Özellikler ve Kullanılan Sass Becerileri

Bu projede kurulan ve sergilenen ileri düzey Sass mimari becerileri şunlardır:

1.  **7-1 Pattern Mimarisinin Uygulanması:** CSS kodunun **`abstracts`**, **`base`** ve **`components`** gibi mantıksal klasörlere ayrılmasıyla mükemmel organizasyon sağlanır.
2.  **Sürdürülebilir Modül Yönetimi (@use):** Modern `@use` kuralı ile parçalar birbirine bağlanır. Bu sayede isim çakışmaları engellenir ve bağımlılıklar açıkça yönetilir.
3.  **Gelişmiş Mixin Kullanımı:**
    * **Tekrarı Önleme (DRY):** `button-size` ve `form-input-base` gibi mixin'ler ile form ve buton stilleri merkezileştirilir.
    * **Responsif Mixin:** `respond-up` mixin'i tanımlanarak, mobil öncelikli responsive tasarım kolayca uygulanır.
4.  **Otomasyon (Programatik Sass):** `@each` döngüsü kullanılarak, sadece bir Sass Haritasına yeni bir renk eklenerek birden fazla renkli kart sınıfı otomatik olarak üretilir.
5.  **Fonksiyonel Renk Yönetimi:** `sass:color` modülü ve `color.adjust()` gibi fonksiyonlar kullanılarak renklerin dinamik olarak (hover gibi durumlarda) koyulaştırılması sağlanır.

---

## 📁 Proje Yapısı (7-1 Pattern)

Projenin modülerliği, aşağıdaki mantıksal klasör yapısıyla sağlanmıştır:

Bu metin, projenizin en güçlü yanlarını (mimari, mixin'ler ve `@use` sistemi) vurgular.


# Sass-Modular-Kit

## Modüler ve Responsif Ön Yüz Başlangıç Kiti

Bu proje, modern web projeleri için tasarlanmış, tamamen modüler (parçalara ayrılmış) ve ölçeklenebilir bir CSS mimarisinin canlı örneğidir. Tüm stiller **Sass (SCSS)** ile yazılmıştır ve endüstri standardı olan **7-1 Pattern** metodolojisini takip eder.

Bu kit, bir projenin büyümesi sırasında kod karmaşasını önlerken, geliştiricilere hız ve sürdürülebilirlik sağlamak için tasarlanmıştır.

---

## 🚀 Temel Özellikler ve Kullanılan Sass Becerileri

Bu projede kurulan ve sergilenen ileri düzey Sass mimari becerileri şunlardır:

1.  **7-1 Pattern Mimarisinin Uygulanması:** CSS kodunun **`abstracts`**, **`base`** ve **`components`** gibi mantıksal klasörlere ayrılmasıyla mükemmel organizasyon sağlanır.
2.  **Sürdürülebilir Modül Yönetimi (@use):** Modern `@use` kuralı ile parçalar birbirine bağlanır. Bu sayede isim çakışmaları engellenir ve bağımlılıklar açıkça yönetilir.
3.  **Gelişmiş Mixin Kullanımı:**
    * **Tekrarı Önleme (DRY):** `button-size` ve `form-input-base` gibi mixin'ler ile form ve buton stilleri merkezileştirilir.
    * **Responsif Mixin:** `respond-up` mixin'i tanımlanarak, mobil öncelikli responsive tasarım kolayca uygulanır.
4.  **Otomasyon (Programatik Sass):** `@each` döngüsü kullanılarak, sadece bir Sass Haritasına yeni bir renk eklenerek birden fazla renkli kart sınıfı otomatik olarak üretilir.
5.  **Fonksiyonel Renk Yönetimi:** `sass:color` modülü ve `color.adjust()` gibi fonksiyonlar kullanılarak renklerin dinamik olarak (hover gibi durumlarda) koyulaştırılması sağlanır.

---

## 📁 Proje Yapısı (7-1 Pattern)

Projenin modülerliği, aşağıdaki mantıksal klasör yapısıyla sağlanmıştır:

```

scss/
├── abstracts/      // Değişkenler, mixin'ler, fonksiyonlar (En temel yardımcılar)
│   ├── \_variables.scss  
│   ├── \_mixins.scss
├── base/          // Proje genelinde uygulanan temel stil kuralları (Reset, Typography)
├── components/    // Bağımsız arayüz bileşenleri (Kartlar, Butonlar, Formlar)
│   ├── \_buttons.scss
│   ├── \_card.scss
│   ├── \_forms.scss
└── style.scss     // Kök dosya (Tüm parçalar burada @use ile birleştirilir)

````

---

## 🛠️ Kurulum ve Kullanım

Bu projeyi yerel ortamınızda çalıştırmak ve geliştirmek için ihtiyacınız olan tek şey Sass derleyicisidir.

1.  **Gerekli Modülü Kurun:**
    ```bash
    npm install -g sass
    ```
2.  **İzlemeyi Başlatın:**
    Projenin kök dizininde aşağıdaki komutu çalıştırarak Sass'ı izlemeye alın. Bu komut, `scss/style.scss` dosyasındaki değişiklikleri otomatik olarak `css/style.css`'e derleyecektir.
    ```bash
    sass --watch scss/style.scss:css/style.css
    ```
3.  **Çalıştırın:**
    `index.html` dosyasını tarayıcınızda açın ve responsive yapının ve bileşenlerin çalıştığını kontrol edin.

