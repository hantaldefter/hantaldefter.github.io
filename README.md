# hantal defter


Bu sitede görmüş olduğunuz bütün kadınlar yazma disiplinlerine ve yaratıcılıklarına hayran olduğum kadınlardır (ve daha niceleri). Burayı birkaç yıldır düşündüğüm bir projeyi hayata geçirmek için, kodlama öğrenme basamağı olarak hazırladım. Bu ilk basamağı adımlarken tek istediğim hayran olduğum kadın yazarların disiplinine ulaşmaktır. Hantal Defter bu sebeple hem görev takibi hem pomodoro olarak tasarlanmıştır ve HTML tabanlı kodlanmıştır. Bütün açık kaynaklara yukarıdaki linklerden ulaşabilirsiniz. Dilediğiniz gibi kullanmakta özgürsünüz. Benimle ezgitspnr99@gmail.com mail adresi üzerinden iletişime geçebilirsiniz ve bu beni çok mutlu eder. Bütün yazma süreçlerinde Ellipsus kullandığım için onlara da köprü oluşturmak istiyorum. Logosuna tıklayarak siteye ulaşabilirsiniz.

Güncellemeler:
20.11.2026 - ayrı aç ve masaüstünde aç olarak iki buton eklendi.

## Nasıl çalışır

- Günde en fazla 5 görev girersin.
- Görevler 45 dakikalık pomodorolarla rastgele karşına çıkar. Biri bitmeden diğerleri görünmez.
- Her biten görev bir yıldız kazandırır. 10 yıldız, dört pomodoro sonrasındaki molaya +5 dakika ek mola hakkı verir (mola 15 dakikadır).
- Mola ve odak başlarken, sayacı durdurmaya çalışırken kedi miyavları çalar.
- Kendi müziklerini (FLAC, MP3, WAV, OGG, M4A, AAC) ekleyip dinleyebilirsin. Dosyalar yalnızca kendi tarayıcında saklanır.
- Sayacı sayfadan ayırıp gezdirebilirsin: **ayrı aç** ve **masaüstü** butonları (aşağıda anlatılıyor).

## Ayrı aç ve masaüstü

Başka sekmelere ya da uygulamalara geçtiğinde de sayacı görebilmen için iki buton var:

- **ayrı aç:** Görev, mod, süre, başlat/durdur, sıfırla ve "bu görevi bitir!" butonlarının olduğu küçük bir pencere açar. Pencerenin boyutunu değiştirdikçe içerik de orantılı olarak büyür ya da küçülür. Document Picture-in-Picture API kullanır.
- **masaüstü:** Tarayıcının video Picture-in-Picture özelliğiyle sayacı küçük bir pencerede gösterir. Bu pencere tarayıcının dışında, diğer uygulamaların üstünde de kalır. Pencere bir görüntü olduğu için butonu yoktur. Medya tuşlarından ⏯ sayacı başlatır/durdurur, ⏭ görevi bitirir.

Notlar:

- İki buton da Chromium tabanlı tarayıcılarda (Chrome, Edge, Opera) çalışır. Firefox, Safari ve telefonlarda butonlar görünmez.
- Sayaç arka plandaki sekmelerde de akıcı kalsın diye Web Worker ile çalışır.
- Masaüstü penceresinde durdurma sırasında kedili "emin misin?" sorusu çıkmaz, çünkü soru ana sekmede kalır ve görünmez.
- Butonlardaki kedi çizimleri `index.html` içine gömülüdür, ayrı dosya gerekmez.

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
