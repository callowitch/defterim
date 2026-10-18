# Defterim — Kurulum Rehberi

Defterim; rutinlerin, bullet journal'ın ve şükür defterin için telefona kurulan bir uygulama. Hiçbir hesaba ya da aboneliğe bağlı değil.

**Yazdıkların nerede duruyor?** Sadece kendi telefonunda. Uygulamanın dosyaları internette yayınlanır, ama senin yazıların ve fotoğrafların hiçbir sunucuya gitmez.

---

## Bu klasördeki dosyalar

| Dosya | Ne işe yarar |
|---|---|
| `index.html` | Uygulamanın kendisi |
| `manifest.webmanifest` | Telefonun onu "uygulama" olarak tanıması için |
| `sw.js` | İnternet yokken de açılması için |
| `icon-*.png`, `apple-touch-icon.png` | Ana ekrandaki simge |
| `KURULUM.md` | Bu rehber (yüklemene gerek yok) |

---

## 1. Ücretsiz bir GitHub hesabı aç

1. **github.com** adresine git ve **Sign up** ile hesap aç.
2. Seçeceğin kullanıcı adı uygulamanın adresinde görünecek. Örneğin kullanıcı adın `hatice` ise adres `https://hatice.github.io/defterim/` olur.

## 2. Uygulama için bir depo oluştur

1. Sağ üstteki **+** düğmesine bas, sonra **New repository**'yi seç.
2. **Repository name** kutusuna `defterim` yaz.
3. **Public** seçili kalsın. Ücretsiz yayın için bu gerekiyor. Burada yalnızca uygulamanın kodu görünür; senin yazıların burada değil, telefonunda durur.
4. **Create repository**'ye bas.

## 3. Dosyaları yükle

1. Açılan sayfada **uploading an existing file** bağlantısına tıkla.
2. Zip'ten çıkardığın klasörün **içindeki** dosyaları (`index.html`, `manifest.webmanifest`, `sw.js` ve png'ler) sürükleyip bırak. Klasörün kendisini değil, içindekileri bırak.
3. Aşağıdaki yeşil **Commit changes** düğmesine bas.

## 4. Yayını aç

1. Deponun üstündeki **Settings** sekmesine gir, soldaki menüden **Pages**'i seç.
2. **Source** için **Deploy from a branch** seçili olsun.
3. **Branch** kısmında `main` ve `/ (root)` seç, **Save**'e bas.
4. 1–2 dakika bekle ve sayfayı yenile. Üstte uygulamanın adresi çıkacak: `https://KULLANICIADIN.github.io/defterim/`

## 5. Telefonuna kur

**iPhone**
1. Adresi **Safari**'de aç. (Chrome'da değil, Safari'de olmalı.)
2. Alttaki **Paylaş** düğmesine (kutudan çıkan ok) bas.
3. **Ana Ekrana Ekle**'yi seç.

**Android**
1. Adresi **Chrome**'da aç.
2. Sağ üstteki **⋮** menüsüne bas.
3. **Uygulamayı yükle** ya da **Ana ekrana ekle**'yi seç.

Artık Defterim ana ekranında. İnternet olmasa da açılır.

> **Önemli (iPhone):** Uygulamayı her zaman **ana ekrandaki simgeden** aç. Safari sekmesinde açtığında kayıtlar ayrı bir yerde tutulur ve simgeden açtığın uygulamada görünmez.

---

## Yedek alma (çok önemli)

Kayıtların telefonunda durduğu için telefonu kaybedersen, uygulamayı silersen ya da tarayıcı verilerini temizlersen kayıtlar da gider. Bunun önlemi basit:

1. Ayda bir uygulamada sağ üstteki **İndir**'e bas.
2. **Yedeği indir (.json)**'a bas. Fotoğraflar da bu dosyanın içinde.
3. Açılan paylaşım menüsünden **Dosyalara Kaydet**, **Google Drive** ya da **iCloud Drive**'ı seç.

Uygulama da 30 günde bir "Yedek zamanı" diye hatırlatır.

**Geri yüklemek için:** Uygulamada **İndir**'e bas, sonra **Yedekten geri yükle**'yi seçip yedek dosyasını göster.

Okumak ya da yazdırmak için **Word** ve **PDF** de indirebilirsin.

---

## Claude'daki Defterim'den taşıma

Claude'daki sürüme bir şey yazdıysan:

1. Claude'daki Defterim'de **İndir**'e bas, sonra **Yedeği indir (.json)**'u seç.
2. Yeni uygulamada **İndir**'e bas, sonra **Yedekten geri yükle**'yi seçip o dosyayı göster.

Yazıların, rutin işaretlerin ve şükür sayfaların gelir. (Yeni uygulamanın yedek dosyasında bunlara ek olarak fotoğraflar, kitap ve film rafın, ay sonu değerlendirmelerin ve kendi eklediğin sorular da bulunur.) Claude sürümündeki fotoğraflar bu dosyaya girmediği için onları yeni uygulamaya tekrar eklemen gerekir.

---

## Daha sonra değişiklik yapmak

1. GitHub'daki depoda değiştirdiğin dosyayı (ör. `index.html`) aynı şekilde yeniden yükle.
2. `sw.js` dosyasının başındaki `defterim-v1` yazısını bir artır (`defterim-v2` gibi) ve onu da yükle. Bu, telefonun yeni sürümü alması için gerekli.
3. Uygulamayı kapatıp iki kez açınca yeni sürüm gelir.

Kayıtların bu güncellemelerden etkilenmez.

## Bilgisayarda hızlıca denemek

`index.html` dosyasına çift tıklarsan tarayıcıda açılır ve çalışır. Ama telefona kurmak ve internetsiz kullanmak için yukarıdaki GitHub adımları gerekli.
