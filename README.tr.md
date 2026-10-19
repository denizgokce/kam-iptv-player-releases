<p align="center">
  <img src="assets/icon.png" width="120" alt="KAM IPTV Player">
</p>

<h1 align="center">KAM IPTV Player</h1>

<p align="center">
  macOS ve Windows için masaüstü IPTV oynatıcısı.<br>
  <b><a href="../../releases/latest">Son sürümü indir</a></b>
</p>

<p align="center">
  <a href="README.md">English</a> · Türkçe · <a href="README.de.md">Deutsch</a>
</p>

---

> **Listeni kendin getir.** KAM IPTV Player yalnızca bir oynatıcıdır. İçinde
> hiçbir kanal, film, dizi, liste ya da sağlayıcı yoktur — kendininkini
> eklersin. [Sorumluluk reddi](DISCLAIMER.tr.md)'ne bak.

Bu depoda **yalnızca kurulum dosyaları** var. Kaynak kodu açık değildir.
Telefon, tablet ve Android TV için [Android için KAM IPTV](https://github.com/denizgokce/kam-iptv-android-releases)'ye bak.

## İndirme

[Son sürümü](../../releases/latest) aç ve bilgisayarına uyan dosyayı seç:

| Dosya | Kimin için |
|---|---|
| `KAM.IPTV.Player-<sürüm>-mac-arm64.dmg` | Apple silicon'lu Mac (M1 ve sonrası) |
| `KAM.IPTV.Player-<sürüm>-mac-x64.dmg` | Intel işlemcili Mac (yayımlandığında) |
| `KAM.IPTV.Player-<sürüm>-win-x64.exe` | Windows 10 / 11, 64 bit |

Her sürümde dosyaların SHA-256 özetleri `SHA256SUMS.txt` içinde.

## Kurulum

### macOS

1. `.dmg` dosyasını aç ve **KAM IPTV Player**'ı **Uygulamalar** klasörüne sürükle.
2. İlk açılışta **uygulamaya sağ tıkla → Aç → Aç**.

Uygulama Apple tarafından onaylanmış (notarize) değil; bu yüzden ilk seferde
çift tıklamak *"Apple denetleyemediği için açılamıyor"* uyarısıyla reddedilir.
Sağ tık → Aç yalnız bir kez gerekir. macOS yine izin vermezse Terminal'de bir
kez şunu çalıştır:

```sh
xattr -dr com.apple.quarantine "/Applications/KAM IPTV Player.app"
```

### Windows

1. `.exe` kurulum dosyasını çalıştır.
2. SmartScreen *"Windows bilgisayarınızı korudu"* derse **Ek bilgi → Yine de çalıştır**'ı seç.

Kurulum dosyası kod imzalı değil; SmartScreen'in sormasının sebebi bu.

## Neler yapıyor

**Listeler**
- Sağlayıcının hesap bilgileriyle (sunucu, kullanıcı adı, parola) giriş yap ya
  da bir M3U / M3U8 dosyası veya adresi yükle.
- Listeler bilgisayarında saklanır ve yalnız sen istediğinde yenilenir.
- **Son Eklenenler** neyin ne zaman geldiğini güne göre gösterir.

**Gezinme**
- Canlı kanallar, filmler ve diziler ayrı bölümlerde; diziler sezonlara kendiliğinden ayrılır.
- Her şeyde arama, yazım hatalarına dayanıklı — ve bir film her adıyla
  bulunur (*A Beautiful Mind* yazınca *Akıl Oyunları* çıkar).
- Kendi **klasör grupların** ve kayıtlı **süzgeç çiplerin** (*HD ama FHD değil*).
- Kendi **oynatma listelerin** — bütün bir seriyi izlemek istediğin sırayla,
  sürükle-bırakla düzenle.
- **İzlediklerim** ve **Favoriler**, kaldığın yerler ve kaldığın kareyle
  *İzlemeye devam et*.

**Bilgiler**
- Ücretsiz Stremio Cinemeta servisinden afiş, konu, puan ve oyuncular.
  Ayarlar'dan tamamen kapatabilirsin; o zaman hiçbir dış servise istek gitmez.

**Oynatma**
- Birkaç oynatma motoru sırayla denenir; diğerlerinin oynatamadığı dosyalar
  (MKV, AVI, alışılmadık kodekler) için yerleşik FFmpeg var.
- Ses ve altyazı seçimi, oynatma hızı, ±10 sn.
- Sen çalışırken üstte kalan yüzen pencerede resim içinde resim.
- Jenerik başladığında başlık izlendi olarak işaretlenir.

## Gizlilik

- Hesap yok, telemetri yok, analitik yok.
- Listelerin, sağlayıcı bilgilerin, favorilerin ve geçmişin bilgisayarında kalır.
- Kendiliğinden bağlanılan tek dış servis Cinemeta'dır, yalnız başlık adlarıyla,
  ve kapatılabilir.

## Sorun bildirme

İşletim sistemini, uygulama sürümünü (Ayarlar) ve ne olduğunu yazarak bir
[issue](../../issues) aç. **Listeni, sağlayıcı adresini, kullanıcı adını ya da
parolanı asla paylaşma** — yayın adresleri bunları içerir.

---

Telif hakkı © 2026 KAM IPTV yazarları. Tüm hakları saklıdır. [LICENSE](LICENSE)
ve [sorumluluk reddi](DISCLAIMER.tr.md).
