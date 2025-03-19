# Sky Torch (Gökyüzü Meşalesi)

## Giriş
Bu eklenti bir YouTube videosu için geliştirilmiştir:
[Minecraft'ta Yörüngesel Lazer (Sky Torch)](https://youtu.be/OKXTGbp6AMk)

## Kurulum
1. JAR dosyasını [sürümler sayfasından](https://github.com/TheCymaera/minecraft-sky-torch/releases/) indirin.
2. [Paper](https://papermc.io/downloads) veya [Spigot](https://getbukkit.org/download/spigot) sunucusu kurun. (Talimatlar aşağıda)
3. İndirdiğiniz JAR dosyasını `plugins` klasörüne ekleyin.
4. [Planet Minecraft](https://www.planetminecraft.com/project/ambertry-forest/) adresinden dünya dosyasını indirin.
   - Bu adım isteğe bağlıdır. Dilediğiniz herhangi bir dünyayı kullanabilirsiniz.
5. İndirdiğiniz dünya klasörünü sunucu dizinine yerleştirin ve adını `world` olarak değiştirin.

## Sunucu Kurulumu
1. [Paper](https://papermc.io/downloads) veya [Spigot](https://getbukkit.org/download/spigot) adresinden sunucu JAR dosyasını indirin.
2. Şu komutu çalıştırın: `java -Xmx1024M -Xms1024M -jar server.jar nogui`
3. Sürüm uyumsuzluklarını önlemek için genellikle Minecraft kurulumunuzla birlikte gelen Java sürümünü kullanmanız önerilir.
   - Modrinth'te, Java kurulum konumunu profil seçenekleri menüsünde bulabilirsiniz.
4. `eula.txt` dosyasındaki `eula=false` değerini `eula=true` olarak değiştirerek lisans sözleşmesini kabul edin.
5. Sunucuya IP adresi olarak `localhost` kullanarak bağlanın.

## Komutlar
Otomatik tamamlama mevcut seçenekleri gösterecektir.
```
# Kontrol öğelerini almak için
/items

# Hazır ayar yüklemek için
/preset <preset:enum>

# Ayarları yeniden yüklemek için (config dosyasını elle düzenledikten sonra)
/reload_config

# Lazerin ölçeğini değiştirmek için
/scale <scale:double>
```

## Geliştirme
1. Depoyu klonlayın veya indirin.
2. Eklentiyi derlemek için Maven `package` komutunu çalıştırın. Oluşturulan JAR dosyası `target` klasöründe olacaktır.
3. Kolaylık için, bir sembolik bağlantı oluşturup bu bağlantıyı sunucunun `plugins` klasörüne ekleyebilirsiniz.
   - Windows için: `mklink /D yeniDosya.jar orijinalDosya.jar`
   - Mac/Linux için: `ln -s orijinalDosya.jar yeniDosya.jar`

## Lisans
Bu eklentiyi ve kaynak kodunu hem ticari hem de ticari olmayan amaçlarla kullanabilirsiniz.

Kaynak belirtmeniz takdir edilir ancak zorunlu değildir.

Önemli değişiklikler yapmadan yeniden satışı yasaktır.
