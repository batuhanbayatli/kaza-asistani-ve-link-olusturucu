# 🚗 Kaza Anı Dijital Asistanı ve Link Oluşturucu (Insurtech Project)

**Küçük ve orta ölçekli sigorta acenteleri için geliştirilmiş, sunucu gerektirmeyen (serverless), kaza anında müşteriyi adım adım yönlendiren mobil web asistanı.**

## 🎯 Projenin Amacı
Sigorta müşterileri kaza anında panik yaşar, ne yapacaklarını unutur ve genellikle eksik evrakla acentelerine dönerler. Bu proje:
1.  **Panik Yönetimi:** Müşteriyi sakinleştirir ve "Triage" (Önceliklendirme) mantığıyla yönlendirir.
2.  **Veri Kaybını Önleme:** Tutanak rehberi **Modal (Popup)** olarak açılır, böylece müşteri sayfadan ayrılmadan yardım alır ve girdiği veriler kaybolmaz.
3.  **Hızlı İletişim:** Konum ve kaza bilgisini tek tuşla acentenin WhatsApp'ına iletir.

## 🚀 Özellikler
* **📱 Mobile First & SPA:** Tamamen mobil cihazlar için optimize edilmiş, sayfa yenilemesi gerektirmeyen Tek Sayfa Uygulama (Single Page Application).
* **📷 Entegre Kamera:** `capture="environment"` özelliği ile uygulama içinden direkt arka kamera açılır.
* **📝 İnteraktif Tutanak Rehberi:** Müşteri takıldığı anda "Nasıl Doldurulur?" butonuna basar, rehber bir pencere (modal) olarak açılır. Örnek doldurulmuş tutanak görseli (`ornek.jpg`) içerir.
* **📍 Geolocation & WhatsApp API:** Koordinatları alır, Google Maps linkine çevirir ve acenteye hazır mesaj taslağı oluşturur.
* **🔒 %100 Gizlilik (Privacy First):** Sunucu veya veritabanı yoktur. Tüm veriler kullanıcının telefonunda işlenir. KVKK/GDPR uyumludur.
* **🔗 Dinamik Link Sistemi:** Acenteler sisteme kaydolmadan, URL parametreleri ile kendilerine özel link oluşturabilirler.

## 🛠️ Nasıl Çalışır?
Sistem temel olarak 3 dosyadan oluşur:

1.  **`olustur.html` (Acente Paneli):**
    * Acente telefon numarasını girer.
    * Sistem, acenteye özel bir link üretir (Örn: `site.com/?tel=90555...`).
    * Acente bu linki müşterisine iletir veya Instagram biosuna ekler.

2.  **`index.html` (Müşteri Asistanı):**
    * Müşteri linke tıkladığında "Kaza Sihirbazı" açılır.
    * Adımlar: Sağlık Kontrolü -> Güvenlik -> Fotoğraflama -> Tutanak -> Gönderim.
    * Rehber ihtiyacında sayfa değişmez, popup açılır.
    * "Gönder" butonuna basıldığında URL'deki numara okunur ve o numaraya WhatsApp mesajı atılır.

3.  **`ornek.jpg` (Asset):**
    * Tutanak rehberi içinde gösterilen örnek kaza tutanağı görselidir.

## 💻 Teknolojiler
Maksimum performans ve uyumluluk için "Vanilla" teknolojiler kullanılmıştır.
* **HTML5** (Semantik yapı, Input Capture)
* **CSS3** (Flexbox, CSS Animations, Responsive Design, Modal Logic)
* **JavaScript (ES6)** (DOM Manipulation, Geolocation API, URLSearchParams)

## ⚠️ Yasal Uyarı
Bu uygulama, sigortacılık süreçlerini kolaylaştırmak amacıyla geliştirilmiş bir **arayüz projesidir**.
* Uygulama acil durum çağrısı (112) yerine geçmez.
* Geliştirici, oluşabilecek maddi hasar veya hukuki süreçlerden sorumlu değildir.
* Veri güvenliği açısından sunucu tabanlı kayıt tutulmamaktadır.

## 👨‍💻 Geliştirici
**Batuhan Bayatlı** *Financial Analyst & InsurTech Developer | Bridging Finance with Data Strategy | Python, SQL & Web | 🇯🇵 🇹🇷

[LinkedIn Profilim](https://www.linkedin.com/in/batuhanbayatlı/)

## 👨‍💻 Geliştirici
**Batuhan Bayatlı** *Insurtech Enthusiast & Front-End Developer* Banking and Insurance Student @ Istanbul Kultur University

[LinkedIn Profilim](https://www.linkedin.com/in/batuhanbayatlı/)
