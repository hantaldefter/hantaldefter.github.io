# hantal defter

DEHB dostu, tek odaklı görev ve pomodoro uygulaması. HTML tabanlıdır, kurulum ya da sunucu gerektirmez.

## Nasıl çalışır

- Günde en fazla 5 görev girersin.
- Görevler 45 dakikalık pomodorolarla rastgele karşına çıkar. Biri bitmeden diğerleri görünmez.
- Her biten görev bir yıldız kazandırır. 10 yıldız, dört pomodoro sonrasındaki molaya +5 dakika ek mola hakkı verir (mola 15 dakikadır).
- Mola ve odak başlarken, sayacı durdurmaya çalışırken kedi miyavları çalar.
- Kendi müziklerini (FLAC, MP3, WAV, OGG, M4A, AAC) ekleyip dinleyebilirsin. Dosyalar yalnızca kendi tarayıcında saklanır.

## Çalıştırma

1. Bu klasördeki dosyaları aynı yapıyla bir arada tut (`index.html`, `assets/`, `fonts/`).
2. `index.html` dosyasını tarayıcıda aç.

GitHub Pages ile yayınlamak için: **Settings → Pages → Branch: main / (root)** seçip kaydet.

## Dosya yapısı

```
index.html      uygulamanın tamamı (HTML, CSS ve JavaScript)
assets/         görseller
assets/sounds/  miyav sesleri
fonts/          Cormorant Garamond İtalik (yazı tipi)
```

## Müzik oynatıcı hakkında

- Yerel müzikler tarayıcının IndexedDB deposunda tutulur, hiçbir yere gönderilmez.
- Spotify özellikleri (gömülü oynatıcı, listeyi içe aktarma) yalnızca `http://` ya da `https://` üzerinden çalışır, dosyayı doğrudan açtığında (`file://`) çalışmaz.
- Spotify'dan parça parça içe aktarmak için kendi Client ID'ni ayarlardan girmelisin.

## Lisans

Lisansı depoya `LICENSE` dosyası olarak ekle (GitHub'da: **Add file → Create new file → LICENSE** yazınca lisans şablonu seçebilirsin).

Görseller, sesler ve yazı tipleri kendi sahiplerine aittir. Depoya eklemeden önce yeniden dağıtım izinlerini kontrol et.
