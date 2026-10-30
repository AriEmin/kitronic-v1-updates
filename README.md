# Kitronic V1 güncellemeleri

Kitronic V1 Android uygulaması ve ESP32 test cihazı için dağıtım deposu. Kaynak proje ve özel imzalama anahtarları bu depoda bulunmaz.

## İndirme ve ilk kurulum

- [Android uygulamasını indir](https://github.com/AriEmin/kitronic-v1-updates/releases/latest/download/Kitronic-Control.apk)
- [ESP32 ilk USB kurulum paketi](https://github.com/AriEmin/kitronic-v1-updates/releases/latest/download/Kitronic-ESP32-USB-1.0.0.zip)
- [Sürümler ve açıklamalar](https://github.com/AriEmin/kitronic-v1-updates/releases)

Android 8 ve üzeri gerekir. İlk OTA destekli ESP sürümü, Classic Bluetooth destekli ESP32 / 4 MB cihaza USB ile yüklenir. USB ZIP'indeki kurulum açıklamasını okuyun. ESP32-S3/C3 için değildir.

Telefon Bluetooth ayarlarında `Kitronic-XXXXXXXXXXXX` cihazını eşleştirin ve uygulamadan bağlanın. Kod fabrika MAC adresinden üretilir. Eski cihaz adı önbellekte kalırsa eşleştirmeyi kaldırıp tekrar eşleştirin.

## Sonraki güncellemeler

Android 4.0.1 bu depoyu varsayılan olarak kullanır. Gerekirse uygulamada **Menü → Güncelleme deposu** alanına `AriEmin/kitronic-v1-updates` girin. **Güncellemeleri kontrol et** ile elle kontrol edilebilir; uygulama açılışında ve Bluetooth bağlantısında otomatik kontrol de yapılır.

Android kurulumu sistem onayıyla tamamlanır. ESP dosyasını telefon indirip Bluetooth ile aktarır; ESP'nin Wi-Fi bağlantısı gerekmez. Güncelleme yalnız ana panelde, işlemler durmuşken başlar. İmza, model, sürüm, boyut ve dosya özeti doğrulanır. Eksik aktarım etkinleştirilmez. OTA sonrasında uygulama aynı cihaza nötr şekilde tekrar bağlanır; test başlatılmaz. Uygulamayı açık tutun. Yeni imaj açılışı 60 saniyede onaylanamazsa geri dönüş istenir.

Makine tarafından okunan imzalı bildirim: `https://github.com/AriEmin/kitronic-v1-updates/releases/latest/download/updates.json`.

## Doğrulama durumu

Yazılım kontrolleri ve emülatör menü testleri geçti. Gerçek ESP üzerinde OTA, enerji kesintisi ve geri dönüş kabul testleri henüz yapılmadı. Son sürümün açıklamaları ve kurulum paketindeki notlar geçerlidir.
