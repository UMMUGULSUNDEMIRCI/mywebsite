# mywebsite
# 📌 Bursa Teknik Üniversitesi Web Sitesi

Bu proje, **Bursa Teknik Üniversitesi** için hazırlanmış bir web sitesi tasarımını içermektedir. HTML, CSS ve JavaScript kullanılarak geliştirilmiş olan bu projede, kullanıcı dostu bir arayüz ve dinamik öğeler bulunmaktadır.

## 🚀 Teknolojiler ve Kullanılan Beceriler

### 1️⃣ **HTML (HyperText Markup Language)**
- Sayfa yapısını oluşturmak için kullanılmıştır.
- Menü, slayt gösterisi, kartlar ve footer gibi temel HTML bileşenleri oluşturulmuştur.
- `<meta>` etiketleri ile mobil uyumluluk sağlanmıştır.

### 2️⃣ **CSS (Cascading Style Sheets)**
- **Dış Stil Dosyası (External CSS)**: `styles.css` dosyasında, web sayfasının genel görünümü belirlenmiştir.
- **FontAwesome Kullanımı**: İkonlar için `FontAwesome` CDN bağlantısı eklenmiştir.
- **Responsive Design (Duyarlı Tasarım)**: `viewport` meta etiketi ile birlikte duyarlı tasarım sağlanmıştır.
- **Hover ve Animasyon Efektleri**: Menü geçişleri ve kart bileşenleri için CSS animasyonları kullanılmıştır.

### 3️⃣ **JavaScript (Dinamik İçerik ve Etkileşim)**
- **Slayt Gösterisi (Slider)**:  
  - `showSlides()` fonksiyonu ile belirli aralıklarla resimler otomatik olarak değişmektedir.
  - `setTimeout()` fonksiyonu ile her 2 saniyede bir slayt değiştirilir.
  - `document.getElementsByClassName("mySlides")` kullanılarak DOM manipülasyonu yapılmıştır.

```javascript
let slideIndex = 0;
showSlides();

function showSlides() {
    let slides = document.getElementsByClassName("mySlides");
    for (let i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
    }
    slideIndex++;
    if (slideIndex > slides.length) { slideIndex = 1 }
    slides[slideIndex - 1].style.display = "block";
    setTimeout(showSlides, 2000);
}
```

- **Dropdown Menü (Alt Menü)**
  - Ana menüde bazı sekmelerin alt menüleri bulunmaktadır.
  - CSS ile `hover` kullanılarak açılır menüler oluşturulmuştur.

- **Harita Entegrasyonu**
  - **Google Maps API** kullanılarak üniversitenin konumu eklenmiştir.
  - `<iframe>` etiketi ile harita gömülmüştür.

- **Sosyal Medya Bağlantıları**
  - Instagram, Twitter ve LinkedIn ikonları eklenmiştir.
  - Kullanıcılar bu ikonlara tıklayarak ilgili sosyal medya hesaplarına yönlendirilebilir.

## 📥 Kurulum ve Çalıştırma

1. Bu projeyi bilgisayarınıza klonlayın:

```bash
git clone https://github.com/kullaniciadi/btu-websitesi.git
```

2. Proje klasörüne girin:

```bash
cd btu-websitesi
```

3. Bir web tarayıcısında `index.html` dosyasını açın.

## 🎯 Özellikler

✅ Duyarlı (Responsive) tasarım  
✅ Dinamik slayt gösterisi  
✅ Açılır (Dropdown) menüler  
✅ Google Maps entegrasyonu  
✅ Sosyal medya bağlantıları  
✅ Bilgi kartları ve tanıtım bölümü  

## 🤝 Katkıda Bulunma

Katkıda bulunmak için:

1. Depoyu forklayın (Fork).
2. Yeni bir dal (branch) oluşturun:
   ```bash
   git checkout -b yeni-ozellik
   ```
3. Değişikliklerinizi yapın ve commitleyin:
   ```bash
   git commit -m "Yeni özellik eklendi"
   ```
4. Değişiklikleri gönderin:
   ```bash
   git push origin yeni-ozellik
   ```
5. Bir **Pull Request (PR)** açın.

## 📄 Not
Sitedeki buton yönlendirmeleri Bursa Teknik Üniversitesinin orijinal web sitesine yapılmıştır.
