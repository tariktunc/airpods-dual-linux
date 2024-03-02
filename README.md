# Apple AirPods'ı Linux'a (Debian/Ubuntu/Mint) Nasıl Bağlanır

## Adım 1.

Terminalinizi açın.

Kök dizininde aşağıdaki komutu çalıştırın:

```bash
sudo nano /etc/bluetooth/main.conf
```

Terminal şifrenizi girmenizi isteyecektir. Lütfen yazın :)

## Adım 2.

Sonrasında, bir terminal penceresinde yapılandırma dosyası açılacaktır.

Şu satırı bulun:

```bash
#ControllerMode = dual
```

## Adım 3.

"dual" olanı "bredr" olarak değiştirin. Son kod şu şekilde olmalıdır:

```bash
ControllerMode = bredr
```

## Adım 4.

Değişiklikleri kaydetmek ve nano editörden çıkmak için şunları yapın:

1. Klavyenizde şu tuşlara basın:

```bash
Ctrl + x
```

2. Nano editörün altında şu soruyu göreceksiniz:

> "Save modified buffer?"

---

3. Klavyenizde şu tuşa basın: y
4. Klavyenizde şu tuşa basın: Enter

Bu adımlardan sonra aynı dizinde normal terminal penceresine geri döneceksiniz.

## Adım 5.

Aşağıdaki komutu terminalde çalıştırın:

```bash
sudo /etc/init.d/bluetooth restart
```

Sonra şu mesajı göreceksiniz:

> "Restarting bluetooth (via systemctl): bluetooth.service."

---

## Adım 6.

Bilgisayar ayarlarına gidin ve Bluetooth'u etkinleştirin, böylece Bluetooth bağlantılarını aramaya başlar

## Adım 7.

Sonraki adımlar tam olarak şu şekilde gerçekleştirilmelidir:

1. AirPods'ları (her ikisini de) kutuya koyun
2. Kapağı açık tutun
3. Kapağı açık ve AirPods'ları kutunun arka tarafındaki düğmeye basılı tutun.
4. Işığın kutunun ön tarafında yanıp sönmesini görene kadar düğmeyi basılı tutun, eşleştirme modunda olduğunu belirten bir ses de yapabilir.

## Adım 8.

Son olarak, tüm bu adımlardan sonra Bluetooth ayarları bölümünde AirPods'ınızı bulmalı ve bağlanmalısınız ;)
