# 🎬 Sinematik

Kişisel film ve dizi takip & öneri sitesi. Tek HTML dosyası, sıfır backend, tamamen ücretsiz.

**[→ sinematik.live](https://rasne-dev.github.io/sinematik)**

---

## Özellikler

- 🔍 **Keşfet** — TMDB üzerinden popüler film & dizi, **çoklu tür seçimi ve puan aralığı filtreleri**, arama, sonsuz kaydırma (infinite scroll).
- ✨ **Öneriler** — Puanlarına göre kişisel öneri motoru (tür ağırlığı + TMDB benzer içerik), **tür ve puan filtreleri**, sonsuz kaydırma.
- 🕐 **İzleme Listesi** — Sonra izlemek istediğin içerikleri kaydet.
- ⭐ **Puanladıklarım** — Tüm puanlarını listele, güncelle, IMDb puanına göre sırala, istatistiklerini gör.
- 📥 **IMDb İçe Aktarma** — IMDb `ratings.csv` dosyasını yükle, tüm puanlar otomatik eşleştirilir.
- 🔞 **İçerik Filtreleme** — Ayarlar kısmından NSFW (yetişkin) içerikleri gizleme ve yaş sınırı ayarı.
- ℹ️ **Akıllı İpucu** — Önerilen içeriklerin neden önerildiğini detay modalında gör.
- 🌙 Dark theme, mobil uyumlu.
- 💾 Tüm veriler tarayıcıda saklanır (localStorage) — kayıt gerekmez.

---

## Kullanım

Doğrudan aç, kurulum gerekmez:

```
index.html → tarayıcıda aç
```

Veya GitHub Pages üzerinden: `rasne-dev.github.io/sinematik`

---

## IMDb Puanlarını İçe Aktarma

1. [imdb.com](https://imdb.com) → Profilim → **Your Ratings** → sağ üst `⋮` → **Export**
2. İndirilen `ratings.csv` dosyasını siteye yükle
3. Tüm puanlar TMDB ile eşleştirilip otomatik içe aktarılır

---

## Teknik

| | |
|---|---|
| Veri kaynağı | [TMDB API](https://www.themoviedb.org/) (ücretsiz) |
| Depolama | `localStorage` (tarayıcı) |
| Bağımlılık | Sıfır — vanilla JS, tek dosya |
| Host | GitHub Pages (ücretsiz) |

---

## Geliştirme Notları

API anahtarı `index.html` içine gömülüdür. TMDB key'leri client-side kullanım için tasarlanmıştır, kısıtlama yaşanırsa [themoviedb.org/settings/api](https://www.themoviedb.org/settings/api) adresinden ücretsiz yeni key alınabilir.

---

## Lisans

MIT © [rasne-dev](https://github.com/rasne-dev)
