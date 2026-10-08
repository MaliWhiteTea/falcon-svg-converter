# KiCad SVG → Falcon Negatif PNG Dönüştürücü

KiCad'den alınan normal SVG çıktısını, Falcon Design Space'te lazerle PCB boya kaldırma işlemi için kullanılabilecek siyah zeminli ve beyaz yollu PNG görüntüsüne dönüştüren çevrimdışı bir araçtır.

## Özellikler

- Kurulum ve internet bağlantısı gerektirmez.
- SVG'nin fiziksel ölçüsünü otomatik okur.
- KiCad'in yaklaşık 0,2 mm Edge.Cuts kenar payını düzeltmeye yardımcı olur.
- Kart ölçüsünü ve çıktı çözünürlüğünü kullanıcıya bırakır.
- 1000, 1270 ve 2540 DPI seçenekleri sunar.
- PNG dosyasına doğru DPI bilgisini ekler.
- Dönüşüm tamamen tarayıcıda yapılır; dosya herhangi bir sunucuya gönderilmez.

## Kullanım

1. `index.html` dosyasını Chrome, Edge veya Firefox ile açın.
2. KiCad'de **Negative plot kapalı** olarak oluşturduğunuz `.svg` dosyasını seçin.
3. Kartın gerçek genişlik ve yüksekliğini kontrol edin.
4. Önizlemede siyah alanların kazınacak, beyaz yolların korunacak bölge olduğunu doğrulayın.
5. **Falcon PNG'sini indir** düğmesine basın.
6. Falcon Design Space'te Görüntü/Dolgu Oyma'yı açın; Çizgi Oyma ve Invert seçeneklerini kapalı tutun.

## KiCad Plot ayarları

Plot alırken ayarlar aşağıdaki gibi olmalıdır:

![KiCad Plot ayarları](assets/kicad-plot-ayarlari.png)

PCB üzerinde gerçek kart ölçülerinde, köşeleri tamamen birleşen kapalı bir `Edge.Cuts` dikdörtgeni bulunmalıdır. `Fit page to board` açık olmalıdır.

## GitHub Pages

Bu depo statik bir web uygulamasıdır. GitHub Pages'i etkinleştirmek için depo ayarlarında **Pages → Deploy from a branch → main / root** seçilebilir.

## Atıf

© Mert Ali AKÇAY — Yapay zeka araçları kullanılarak tasarlanmıştır.
