# 🎬 Sinematik

Sinematik, modern bir arayüze sahip, tamamen tarayıcı üzerinde çalışan (serverless) kişisel bir film ve dizi takip platformudur. Kayıt gerektirmez, verilerinizi yerel olarak saklar ve size özel bir sinema kütüphanesi sunar.

### 🔗 [Uygulamayı Aç](https://rasne-dev.github.io/Sinematik/)

---

## 🚀 Öne Çıkan Özellikler

### 🔍 Akıllı Keşfet & Filtreleme
- **Dinamik Kategoriler:** Sayfayı her açtığınızda *Popüler, En Yüksek Puanlı, Yeni Vizyona Girenler* gibi farklı kategorilerle karşılaşırsınız.
- **Gelişmiş Filtreleme:** Hem Keşfet hem de Öneriler kısmında **çoklu tür seçimi** (Aksiyon + Komedi) ve minimum puan filtresi.
- **Anlık Arama:** `AbortController` desteğiyle yarış durumlarını önleyen hızlı arama motoru.

### ✨ Kişisel Öneri Motoru
- **Rastgele Bazlı Çeşitlilik:** Puanladığınız içerikler arasından her seferinde farklı kaynaklar seçilerek sunulan taze öneriler.
- **İlişkisel Analiz:** Sevdiğiniz bir filmin "Neden Önerildiğini" anında görün.

### ⭐ Modern Puanlama ve Takip
- **Otomatik Kayıt:** Yıldızlara tıkladığınız an puanınız kaydedilir, "Kaydet" butonuyla uğraşmanıza gerek kalmaz.
- **Yıldız Sayacı:** Puan verirken kaçıncı yıldızda olduğunuzu gösteren (8/10) dinamik gösterge.
- **Toggle-Off:** Yanlışlıkla verdiğiniz puanı aynı yıldıza tekrar tıklayarak silebilirsiniz.
- **Hızlı İzleme Listesi:** Film kartlarının üzerine gelerek (hover) detaya girmeden tek tıkla listeye ekleme/çıkarma.

### 🍿 IMDb & OMDb Entegrasyonu
- **Kartlarda IMDb Puanı:** OMDb API desteğiyle film kartlarının üzerinde gerçek IMDb puanlarını görün.
- **YouTube Fragmanları:** Detay panelinde tek tıkla resmi fragmanlara erişim.
- **Gelişmiş İçe Aktarma:** IMDb `ratings.csv` dosyasını sürükle-bırak yöntemiyle saniyeler içinde kütüphanenize dahil edin.

### 🎭 UX/UI İyileştirmeleri
- **Etkileşimli Oyuncular:** Oyuncu profillerine tıklayarak o oyuncunun tüm filmografisini anında aratın.
- **Gelişmiş Görsel Hiyerarşi:** Aksiyon, Dram, Korku gibi türler için özel renkli etiketler.
- **Akıllı Navigasyon:** Sayfa aşağı kaydırıldığında çıkan "Başa Dön" butonu ve genişletilmiş (200px) film özetleri.

---

## 🛠️ Teknik Detaylar

| Bileşen | Teknoloji |
|---|---|
| **Frontend** | Vanilla JS (ES6+), CSS3 (Custom Variables), HTML5 |
| **Veri Kaynağı** | [TMDB API](https://www.themoviedb.org/) & [OMDb API](https://www.omdbapi.com/) |
| **Depolama** | `localStorage` (Kayıt gerektirmez, %100 gizlilik) |
| **Performans** | Tek dosya, sıfır bağımlılık, anlık yükleme |

---

## 📖 Kullanım Kılavuzu

### API Anahtarları Hakkında
Uygulama varsayılan bir TMDB anahtarıyla gelir. Ancak gerçek IMDb puanlarını görmek için:
1. [omdbapi.com](https://www.omdbapi.com/apikey.aspx) adresinden ücretsiz bir anahtar alın.
2. Sinematik içinde **Ayarlar (⚙️)** menüsüne girip anahtarı kaydedin.

### IMDb Puanlarını Aktarma
1. [imdb.com](https://imdb.com) → Profilim → **Your Ratings** → sağ üst `⋮` → **Export** yolunu izleyin.
2. İndirilen `ratings.csv` dosyasını uygulamadaki **"IMDb İçe Aktar"** butonuna tıklayarak yükleyin.
3. Uygulama, IMDb ID'lerini kullanarak tüm içerikleri otomatik olarak TMDB verileriyle eşleştirir.

### 💾 Yedekleme & Geri Yükleme
- Sinematik içindeki tüm verilerinizi (puanlar, izleme listesi, ayarlar) tek bir JSON dosyası olarak dışa aktarabilirsiniz.
- Dışa aktardığınız dosyayı daha sonra "Ayarlar" menüsünden geri yükleyerek tüm verilerinizi geri getirebilirsiniz. Bu özellik, tarayıcı değiştirirken veya veri kaybı endişesi yaşadığınızda büyük kolaylık sağlar.

---

## 📜 Lisans
MIT © [rasne-dev](https://github.com/rasne-dev)
