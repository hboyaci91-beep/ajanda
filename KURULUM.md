# İş Takip — Tablete Kurulum

Bu uygulama tablette kendi simgesiyle, ayrı bir uygulama gibi çalışır. Hesap ya da şifre istemez, kurulduktan sonra internetsiz de çalışır. **Kayıtlarınız yalnızca tablette saklanır, hiçbir sunucuya gönderilmez.**

Kurulum iki adımdır: (1) dosyaları bir kez ücretsiz bir web adresine koymak, (2) o adresi tablette açıp ana ekrana eklemek. İlk adım için yaklaşık 10 dakika ayırın; bir kez yapılır.

> Web adresinde yalnızca boş uygulama durur. Sizin girdiğiniz işler, notlar ve personel bilgileri oraya gitmez.

---

## 1. Adım — Dosyaları ücretsiz bir adrese koymak (GitHub Pages)

Bunu bilgisayardan yapmak daha kolaydır. Kurum ağı GitHub'ı engelliyorsa evden yapın.

1. **https://github.com** adresine gidin, **Sign up** ile ücretsiz bir hesap açın.
2. Sağ üstteki **+** işaretine dokunun → **New repository**.
   - Repository name: `is-takip`
   - **Public** seçili kalsın.
   - **Create repository** düğmesine basın.
3. Açılan sayfada **"uploading an existing file"** bağlantısına tıklayın.
4. Bu klasördeki şu **6 dosyayı** sürükleyip bırakın:
   `index.html`, `sw.js`, `manifest.webmanifest`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`
   Ardından alttaki **Commit changes** düğmesine basın.
5. Üstteki **Settings** sekmesi → soldaki menüden **Pages**.
   - **Source:** Deploy from a branch
   - **Branch:** `main`, klasör `/ (root)` → **Save**
6. 1–2 dakika bekleyin. Sayfanın üstünde adresiniz görünür:
   **`https://KULLANICIADINIZ.github.io/is-takip/`**

Bu adresi not edin.

---

## 2. Adım — Tablete kurmak

### iPad
1. Adresi **Safari** ile açın (Chrome değil).
2. Üstteki **Paylaş** düğmesine (yukarı ok olan kare) dokunun → **Ana Ekrana Ekle** → **Ekle**.
3. Ana ekranda kırmızı **İş Takip** simgesi belirir. **Bundan sonra uygulamayı hep bu simgeden açın.**

> Önemli: iPad'de Safari sekmesi ile ana ekrandaki simge ayrı hafıza kullanır. Kayıtlarınızı hep simgeden açtığınız uygulamaya girin; Safari sekmesine girdikleriniz simgede görünmez.

### Android tablet
1. Adresi **Chrome** ile açın.
2. Sağ üstteki **⋮** menüsü → **Uygulamayı yükle** (ya da **Ana ekrana ekle**) → **Yükle**.
3. Uygulama, diğer uygulamalarınızın arasında **İş Takip** adıyla görünür.

İlk açılışta grup başkanlıklarınızın adlarını yazmanızı ister. Sonrasında internet olmadan da çalışır.

---

## Kullanım

- **Ana ekran:** Üstte **İş Takibi** ve **Bilgi Notları** sekmeleri, altında solda **Bugün** kartı (son günü gelen/geçen ve takip günü gelen işler), sağda **Notlarım ve hatırlatmalarım** kutusu, ardından grup başkanlığı kartları.
- **Grup sayfası:** İşler tablo halinde alt alta. **Satır ekle** ile yeni iş yazılır; aynı satıra açıklama, **alt işler**, **belgeler**, **son gün** ve **takip tarihi** girilir. Soldaki kutu işaretlenince iş tamamlanır ve yeşil olarak yerinde kalır. Tablo sağa sola kaydırılır; iş adı solda sabit kalır.
- **Detay:** Satırdaki "Detay" ile not ekleme, öncelik, personel, birden fazla grup seçme ve evrak bilgisi.
- **Personel filtresi ve arama:** Grup sayfasının üstünde.
- **İndir:** Her listede "İndir" ile tablo **PDF** ya da **Word (.docx)** olarak alınır.
- **Bilgi Notları:** Evraklar doğrudan ya da klasörlere yüklenir; dosya ekrana sürüklenerek de yüklenebilir.
- **Görünüm boyutu:** "− 100% +" ile küçültüp büyütün; grup sayfalarında "Sığdır" tabloyu ekrana sığdırır. Beğendiğiniz boyutu Ayarlar'dan "%100" yapabilirsiniz.
- **Ayarlar:** Gruplar (ad, renk, anahtar kelime), personel (grup grup), **PIN**, görünüm boyutu, uyarı süresi, yedek.
- **PIN:** Açılışta ve 1 dakikadan uzun süre kapalı kalınca sorulur. Unutulursa kurtarılamaz; uygulama sıfırlanıp yedekten geri yüklenir.
- Uyarılar uygulamayı açtığınızda görünür; uygulama kapalıyken bildirim göndermez.

## Yedek (çok önemli)

Kayıtlar yalnızca tablette olduğu için, tablet bozulur ya da uygulama silinirse kayıtlar gider.

- **Ayarlar ve yedek → Yedek al:** iPad'de paylaşım menüsü açılır; **Dosyalar'a Kaydet**, e-posta ya da AirDrop ile saklayın. Android'de dosya İndirilenler klasörüne iner.
- Uygulama 7 günden uzun süre yedek alınmazsa ekranın üstünde hatırlatır. Haftada bir yedek alın.
- **Yedekten geri yükle:** Yeni tablete geçerken ya da bir sorun olduğunda yedek dosyasını seçin. (Cihazdaki mevcut kayıtların yerini alır.)
- Yedek dosyasını bilgisayarınızda da açabilirsiniz: aynı adresi bilgisayarın tarayıcısında açıp **Yedekten geri yükle** ile kayıtlarınızı orada görebilirsiniz. (İki cihaz otomatik eşleşmez; hangisinde çalışıyorsanız ondan yedek alıp diğerine yüklersiniz.)

---

## Güncelleme

Uygulamada bir değişiklik yapıldığında yeni `index.html` dosyasını GitHub'daki aynı yere yükleyin ve `sw.js` içindeki `is-takip-v1` sürüm adını bir artırın (`is-takip-v2`). Tablet internete bağlandığında yeni sürümü kendisi alır; kayıtlarınız silinmez.
