# 🚗 Kaza Anı Dijital Asistanı ve Link Oluşturucu (Insurtech Project)

**Küçük ve orta ölçekli sigorta acenteleri için geliştirilmiş, sunucu gerektirmeyen (serverless), kaza anında müşteriyi adım adım yönlendiren mobil web asistanı.**

## 🎯 Projenin Amacı
Sigorta müşterileri kaza anında panik yaşar, ne yapacaklarını unutur ve genellikle eksik evrak/fotoğraf ile acentelerine dönerler. Bu proje:
1.  **Panik Yönetimi:** Müşteriyi sakinleştirir ve adım adım (Triage) yönlendirir.
2.  **Eksik Evrak Önleme:** Fotoğraf ve evrak checklist'i sunar.
3.  **Hızlı İletişim:** Konum ve kaza bilgisini tek tuşla acentenin WhatsApp'ına iletir.

## 🚀 Özellikler
* **📱 Mobile First Tasarım:** Tamamen mobil cihazlar için optimize edilmiş UI/UX.
* **📷 Entegre Kamera:** `capture="environment"` özelliği ile uygulama içinden direkt arka kamera açılır.
* **📍 Geolocation & WhatsApp API:** Koordinatları alır, Google Maps linkine çevirir ve acenteye mesaj taslağı oluşturur.
* **🔒 %100 Gizlilik (Privacy First):** Sunucu veya veritabanı yoktur. Tüm veriler (fotoğraf, konum) kullanıcının telefonunda işlenir. KVKK sorunu yaratmaz.
* **🔗 Dinamik Link Sistemi:** Acenteler sisteme kaydolmadan, sadece URL parametreleri ile kendilerine özel link oluşturabilirler.

## 🛠️ Nasıl Çalışır?
Sistem iki ana dosyadan oluşur:

1.  **`olustur.html` (Acente Paneli):**
    * Acente telefon numarasını girer.
    * Sistem, acenteye özel bir link üretir (Örn: `site.com/?tel=90555...`).
    * Acente bu linki müşterisine iletir.

2.  **`index.html` (Müşteri Asistanı):**
    * Müşteri linke tıkladığında "Kaza Sihirbazı" açılır.
    * Adımlar: Sağlık Kontrolü -> Güvenlik Önlemleri -> Fotoğraflama -> Tutanak -> Gönderim.
    * "Gönder" butonuna basıldığında, URL'deki numara okunur ve o numaraya WhatsApp mesajı atılır.

## 💻 Teknolojiler
Bu proje, maksimum performans ve uyumluluk için "Vanilla" teknolojilerle yazılmıştır.
* **HTML5** (Semantik yapı ve Input Capture özellikleri)
* **CSS3** (Responsive tasarım, Flexbox, Animasyonlar)
* **JavaScript (ES6)** (DOM manipülasyonu, Geolocation API, URLSearchParams)

## ⚠️ Yasal Uyarı ve Sorumluluk Reddi
Bu uygulama, sigortacılık süreçlerini kolaylaştırmak amacıyla geliştirilmiş bir **arayüz projesidir**.
* Uygulama acil durum çağrısı (112) yerine geçmez.
* Geliştirici, oluşabilecek maddi hasar veya hukuki süreçlerden sorumlu değildir.
* Veri güvenliği açısından sunucu tabanlı kayıt tutulmamaktadır.

## 👨‍💻 Geliştirici
**Batuhan Bayatlı** *Insurtech Enthusiast & Front-End Developer* Banking and Insurance Student @ Istanbul Kultur University

[LinkedIn Profilim](https://www.linkedin.com/in/batuhanbayatlı/)
