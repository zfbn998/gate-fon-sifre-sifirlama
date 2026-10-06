# gate io fon şifresi: Unuttuğunuzda nasıl sıfırlanır, kaldırma nasıl yapılır ve 24 saatlik çekim kilidi neden gelir

Türkiye'den Gate kullananların en sık takıldığı yer aynı: USDT çekmeye çalışıyorsunuz, karşınıza "fon şifresi" diye bir alan çıkıyor ve böyle bir şifre belirlediğinizi hatırlamıyorsunuz. Birkaç denemeden sonra "fon şifresi yanlış" uyarısı geliyor. Sıfırlamaya kalktığınızda bu kez takma ad hatası ya da 24 saatlik çekim engeli çıkıyor. Bu yazıda fon şifresinin ne olduğunu, nerede ayarlandığını, unutulduğunda hangi adımların işe yaradığını ve o meşhur 24 saatlik bekleme süresinin neden geldiğini sırayla anlatıyorum.

## Fon şifresi aslında ne işe yarıyor?

Gate hesabında birbirinden bağımsız iki şifre var. Giriş şifresi hesabın kapısını açar. Fon şifresi ise o kapının arkasındaki varlıkları hareket ettirmek için gereken ikinci anahtar.

Gate'in kendi yardım dokümanı fon şifresini hesap güvenliği için kritik bir doğrulama adımı olarak tanımlıyor ve altını çizdiği nokta şu: tüm kişisel verileriniz çalınsa, telefonunuz ele geçirilse bile fon şifresi olmadan varlıklarınız satılamaz veya transfer edilemez.

Bu yüzden fon şifresi genelde şu işlemlerde karşınıza çıkar:

- Kripto para çekme talebi oluştururken
- Fiat/C2C tarafında satış yaparken
- API anahtarı oluştururken (üçüncü taraf entegrasyon dokümanları da bunu not düşüyor)
- Hesap güvenlik ayarlarında fon şifresiyle ilgili bir değişiklik yaparken

Alım satım tarafında her emirde şifre sorulması zorunlu değil. Bu, seçtiğiniz "giriş sıklığı" ayarına bağlı; o ayarın nasıl çalıştığını aşağıda ayrı bir başlıkta anlatıyorum.

## Fon şifresi belirleme: web üzerinden adım adım

Web'den işlem yapıyorsanız süreç yaklaşık 2-3 dakika sürüyor:

1. Sağ üst köşedeki profil (avatar) simgesine tıklayın.
2. Açılan menüden **Güvenlik Ayarları** seçeneğine girin.
3. Sayfayı aşağı kaydırıp **Şifre Yönetimi** başlığı altındaki **Fon Şifresi** satırını bulun.
4. Sağdaki **Değiştir** butonuna tıklayın. Daha önce hiç şifre belirlemediyseniz bu ekran sizi doğrudan belirleme akışına alır.
5. Yeni şifrenizi girin, doğrulama için tekrar yazın.
6. E-posta adresinize gelen doğrulama kodunu ilgili alana girin ve onaylayın.

Onaydan sonra fon şifresi aktif hale gelir. Eğer Google Authenticator bağlıysa doğrulama adımlarında onu da isteyecektir.

## Uygulamadan (APP) belirleme

Mobilde menü yapısı biraz farklı, o yüzden karıştırılıyor:

1. Sol üstteki profil alanına dokunun.
2. Açılan ekranda **Güvenlik** sekmesine geçin.
3. Sayfayı biraz kaydırıp **Temel Güvenlik** başlığındaki **Fon Şifresi** satırına dokunun.
4. Şifreyi belirleyin, tekrar girip e-postanıza gelen kodu yazın ve onaylayın.

Aynı ayar, "Profil ve Ayarlar" → "Güvenlik Merkezi" → "Fon Şifresi" yolu üzerinden de bulunabiliyor. Gate arayüzü zaman zaman menü isimlerini güncelliyor; hangi sürümü kullanırsanız kullanın aradığınız yer her zaman güvenlik ayarları altındaki "şifre yönetimi" bölümü.

## Şifrenin uyması gereken kurallar

Fon şifresi belirlerken sistem sizi şu kalıba sokuyor:

- 8-30 karakter uzunluğunda olmalı
- En az bir büyük harf (A-Z)
- En az bir küçük harf (a-z)
- En az bir rakam (0-9)
- Giriş şifrenizle aynı ya da ona çok benzeyen bir şifre kabul edilmiyor

Son madde pratikte birçok kişiyi yavaşlatıyor: "Kripto123" gibi bir şifreyi giriş şifresi olarak da fon şifresi olarak da kullanmayı denerseniz sistem reddediyor. Ayrıca şifreyi telefonunuza not olarak kaydetmeyin; Gate bunu özellikle vurguluyor. Tek seferlik bir kod üreteciniz yoksa en makul yöntem, parola yöneticisi kullanmak.

## Fon şifresi giriş sıklığı: bir saat / her seferinde / asla

Şifre yönetimi bölümünde "Fon Şifresi" satırının sağındaki küçük ok simgesine tıklarsanız üç seçenek görürsünüz:

| Seçenek | Ne yapıyor | Kim için mantıklı |
| --- | --- | --- |
| Bir saat / Saatlik | Şifreyi girdikten sonra bir saat boyunca tekrar sormaz | Sık işlem yapan, sürekli al-sat yapan kullanıcılar |
| Her seferinde | Her kritik işlemde şifreyi yeniden ister | Hesabını nadiren kullanan, güvenliği önceleyen kullanıcılar |
| Asla | Fon şifresi doğrulamasını devre dışı bırakır | Sadece küçük test işlemleri yapanlar; uzun vadede önerilmez |

Web'de bu ayarı değiştirmek için fon şifrenizi ve Google doğrulama kodunuzu girmeniz istenir. Uygulamada ise fon şifresi sayfasındaki **Giriş Sıklığı** seçeneğinden aynı ayarı yapabilirsiniz.

"Ayarları değiştirmek yeni bir 24 saat kilidi başlatır mı?" sorusu burada haklı bir endişe. Sıklık ayarını değiştirmek fon şifresini sıfırlamakla aynı işlem değil, ama ekranın size gösterdiği uyarıyı okumadan onaylamayın; hesap güvenlik ayarlarındaki her değişiklik sonrası Gate'nin ne yazdığını yalnızca sizin hesabınız gösterir.

## Fon şifresini unuttuysanız: sıfırlama akışı

Panik yapmayı gerektiren bir durum yok, sıfırlama tamamen self-servis yapılabiliyor. Web'de:

1. Güvenlik Ayarları → Şifre Yönetimi → Fon Şifresi bölümüne gidin.
2. **Değiştir** yanındaki akıştan **Şifremi unuttum** bağlantısına tıklayın.
3. E-posta ya da telefon numarası ile sıfırlama yöntemini seçin.
4. Gelen doğrulama kodunu girin.
5. Yeni fon şifresini belirleyip onaylayın.

Uygulamada ise Güvenlik Merkezi → Fon Şifresi ekranında "Şifreyi sıfırla" seçeneği bulunuyor. Eski sürüm Gate duyurularında sıfırlamanın yalnızca web'den yapılabildiği yazıyordu; güncel yardım dokümanları hem web hem uygulama üzerinden sıfırlamaya izin veriyor, o yüzden mobildeyseniz önce uygulamadan deneyin.

Sıfırlama sırasında istenen doğrulama yöntemi hesabınızın durumuna göre değişir: e-posta kodu, SMS kodu ve bağlıysa Google Authenticator kodu. Bazı hesap durumlarında süreç ek doğrulama adımlarına ve manuel incelemeye düşebiliyor; bu durumda kayıtlı e-postanıza gelen yönlendirmeleri takip etmeniz gerekiyor.

### "Takma ad yanlış" ya da "kullanıcı adı yok" hatası

Sıfırlama ekranında en can sıkıcı hata bu. Türkçe forumlarda (R10 gibi) aynı sorunu yaşayan kullanıcıların paylaştığı çözümler şöyle:

- Kullanıcı adı alanına e-posta yerine **kayıtlı telefon numaranızı** yazmayı deneyin.
- Alanı tamamen boş bırakıp yalnızca e-posta ve giriş şifresiyle ilerlemeyi deneyin.
- Tarayıcıyı **gizli sekmede** açın. Sorunun çoğu zaman eski çerezlerden kaynaklandığını bildiren kullanıcılar var.

Bunlar resmi bir Gate talimatı değil, kullanıcı deneyimi. Yine de işe yaradığı yönünde yeterince geri bildirim var.

## Sıfırlama sonrası 24 saatlik çekim kilidi

İşin en çok kafa karıştıran kısmı burası. Fon şifrenizi sıfırladıktan sonra çekim yapmayı denerseniz şu mesajla karşılaşırsınız: hesap güvenlik ayarlarında bir değişiklik algılandı ve koruma amacıyla çekimler 24 saat devre dışı bırakıldı.

Öne çıkan detaylar:

- Kısıtlama **para çekme** ve **fiat/C2C işlemlerini** kapsıyor. Diğer alım satım işlemleri etkilenmiyor.
- Bu 24 saatlik pencere **kaldırılamıyor**. Gate bunu pazarlık konusu olmayan bir güvenlik önlemi olarak tanımlıyor: hesabı ele geçiren biri ayarı değiştirdiyse gerçek sahibinin durumu fark edip müdahale edebilmesi için tanınan süre.
- Sadece fon şifresi değil, giriş şifresi sıfırlama ve iki adımlı doğrulama (2FA) değişiklikleri de aynı kilidi tetikliyor.
- Değişikliğin tam olarak ne zaman yapıldığını **Giriş Geçmişi** (Login History) ve güvenlik kayıtları ekranından görebilirsiniz.

Yani 35 USDT çekmek için iki gün uğraştığını anlatan Technopat üyeleri paranoyak değil; sadece arka arkaya iki kez güvenlik ayarı değiştirdikleri için sayacı iki kez sıfırlamışlar. Önce tüm ayarları (2FA, SMS doğrulama, fon şifresi) tamamlayın, sonra tek seferde bekleyin. Parça parça ilerlemek süreyi uzatmaktan başka işe yaramıyor.

> Not: Bazı üçüncü taraf siteler bu süreyi 72 saat olarak yazıyor. Gate'in kendi yardım merkezi ve Gate TR destek sayfaları 24 saat diyor; resmi kaynak olarak 24 saati esas alın.

## Fon şifresini kaldırabilir miyim?

Şifre ayarlarının yanında "Değiştir" ile birlikte bir **devre dışı bırakma / kaldırma** seçeneği de bulunuyor. Teknik olarak mümkün.

Ama mantıklı mı, orası tartışılır. Fon şifresi tam olarak hesabınız ele geçirildiğinde parayı çıkış kapısında durdurmak için var. Onu kapatmak, kilitli kasayı açık bırakmaya benziyor. Şifreyi hatırlamakta zorlanıyorsanız kaldırmak yerine giriş sıklığını "bir saat" yapmak çok daha makul bir çözüm: hem her işlemde yazmazsınız hem de koruma yerinde kalır.

Kaldırma işleminin çekimler üzerindeki etkisi, hangi ekrandan yaptığınıza ve hesabınızın durumuna göre değişebiliyor. İşlemi onaylamadan önce ekranda çıkan uyarıyı sonuna kadar okuyun; kaldırma sonrası ne kadar süre çekim yapamayacağınız orada yazıyor.

## Gate Web3 cüzdan fon şifresi aynı şifre değil

Bu ayrımı atlayan çok kişi var ve sonucu ağır olabiliyor. Gate borsasındaki fon şifresi ile Gate Web3 cüzdanındaki fon şifresi/kilitleme şifresi/bulut yedekleme şifresi ayrı şeyler:

- Cüzdan şifreleri **yerel veri şifrelemesi** için kullanılıyor. Borsadaki fon şifrenizi değiştirdiğinizde cüzdandaki şifre otomatik olarak güncellenmiyor.
- Cüzdan şifresini değiştirmek istiyorsanız önce **kurtarma ifadenizi (seed phrase) veya özel anahtarınızı** yedeklediğinizden emin olun; ardından cüzdanı sıfırlayıp yeni Gate fon şifresiyle yeniden içe aktarırsınız. Bu işlemden sonra cüzdan şifresi yeni belirlediğiniz şifreyle uyumlu hale gelir.
- Web3 tarafının acı gerçeği şu: kurtarma ifadenizi yedeklememişseniz ve cüzdan şifresini de unuttuysanız, o cüzdandaki varlıklar kurtarılamaz. Merkezi bir borsa değil, zincir üstü bir cüzdan olduğu için geri dönüş mekanizması yok.

Kısacası: borsadaki fon şifresini sıfırlamak Web3 cüzdanınızı kurtarmaz. Cüzdanla işiniz varsa kurtarma ifadesi yedeklemesi şifreden önce gelir.

## Fon şifresi, API anahtarı ve VIP seviyesi ilişkisi

API üzerinden işlem yapanlar için küçük bir not: birçok üçüncü taraf aracın entegrasyon dokümanı, API anahtarı oluştururken fon şifresi belirlemenizin istenebileceğini belirtiyor. Okuma yetkili (read-only) bir anahtar için bile hesap ayarlarında fon şifresi tanımlı olması gerekebiliyor.

Fon şifresi hesabınızın güvenlik katmanı; komisyon seviyesi ise tamamen farklı bir mekanizma. Yine de ikisi aynı hesapta buluştuğu için Gate'in güncel ücret yapısına bakmakta fayda var. Gate, 9 Nisan 2026'da spot ve vadeli işlem komisyon yapısını güncelledi; VIP0 ila VIP2 seviyelerinde oranlar sabit kaldı, üst seviyelerde GT indirimleri güçlendirildi.

VIP seviyesi iki kriterden **yüksek olanına** göre belirleniyor: son 30 günlük toplam işlem hacmi ya da 14 günlük ortalama GT varlığı. 30 günlük hacim hesabına spot ve hisse işlemleri tam, vadeli işlemler %40, USD1 vadeli %20, opsiyonlar %20, CFD'ler %10 ağırlıkla giriyor.

| Seviye | 30 günlük spot hacmi (USD) | VIP yükseltme için varlık (USD) | Maker / Taker | GT ile ödeme (Maker / Taker) | Kayıt |
| --- | --- | --- | --- | --- | --- |
| VIP0 | 0 | 0 | 0,10% / 0,10% | 0,09% / 0,09% | [Gate hesabı aç](https://bit.ly/GateVIP) |
| VIP1 | 60.000 | 2.000 | 0,099% / 0,099% | 0,089% / 0,089% | [VIP1 seviyesiyle başla](https://bit.ly/GateVIP) |
| VIP2 | 120.000 | 4.000 | 0,098% / 0,098% | 0,088% / 0,088% | [VIP2 hesabı oluştur](https://bit.ly/GateVIP) |
| VIP3 | 240.000 | 10.000 | 0,097% / 0,097% | 0,087% / 0,087% | [Gate'e kayıt ol](https://bit.ly/GateVIP) |
| VIP4 | 500.000 | 20.000 | 0,095% / 0,096% | 0,086% / 0,086% | [VIP4 avantajlarını gör](https://bit.ly/GateVIP) |
| VIP5 | 1.000.000 | 40.000 | 0,09% / 0,095% | 0,081% / 0,085% | [Hesabını aç](https://bit.ly/GateVIP) |
| VIP6 | 3.000.000 | 100.000 | 0,085% / 0,09% | 0,076% / 0,081% | [VIP6 seviyesine geç](https://bit.ly/GateVIP) |
| VIP7 | 8.000.000 | 200.000 | 0,08% / 0,085% | 0,07% / 0,076% | [Gate kaydını tamamla](https://bit.ly/GateVIP) |
| VIP8 | 20.000.000 | 400.000 | 0,075% / 0,08% | 0,06% / 0,072% | [VIP8 seçeneklerini incele](https://bit.ly/GateVIP) |
| VIP9 | 50.000.000 | — | 0,07% / 0,075% | 0,05% / 0,068% | [Gate hesabı oluştur](https://bit.ly/GateVIP) |
| VIP10 | 100.000.000 | 2.000.000 | 0,04% / 0,058% | 0,04% / 0,058% | [Hemen kayıt ol](https://bit.ly/GateVIP) |
| VIP11 | 120.000.000 | 4.000.000 | 0,03% / 0,045% | — | [Kayıt sayfasına git](https://bit.ly/GateVIP) |
| VIP12 | 240.000.000 | 8.000.000 | 0,02% / 0,037% | — | [Gate üyeliği aç](https://bit.ly/GateVIP) |
| VIP13 | 440.000.000 | 16.000.000 | 0,01% / 0,03% | — | [VIP başvurusu yap](https://bit.ly/GateVIP) |
| VIP14 | 800.000.000 | 30.000.000 | 0,008% / 0,023% | — | [Gate hesabı aç](https://bit.ly/GateVIP) |
| VIP15 | 1.600.000.000 | 60.000.000 | 0% / 0,02% | — | [Seviye detaylarını gör](https://bit.ly/GateVIP) |
| VIP16 | 3.000.000.000 | 100.000.000 | 0% / 0,0175% | 0% / 0,0175% | [En üst VIP seviyesi](https://bit.ly/GateVIP) |

Komisyon oranları ve seviye eşikleri Gate tarafından dönem dönem güncelleniyor; işlem yapmadan önce hesabınızdaki güncel oran tablosunu ve VIP sayfasını kontrol edin. Tablodaki "—" olan hücreler, ilgili kaynakta açıkça belirtilmeyen değerlerdir. Bu seviyeler satın alınan paketler değil, hesap aktivitenize göre otomatik açılan kademeler; o yüzden kayıt tek noktadan yapılıyor 👉 [hesap açma sayfasına buradan ulaşabilirsiniz](https://bit.ly/GateVIP).

## Sık sorulan sorular

**Fon şifremi unuttum, hesabıma erişemiyor muyum?**
Hayır. Fon şifresi girişi engellemiyor, sadece hassas işlemleri durduruyor. Hesabınıza normal giriş yapıp güvenlik ayarlarından sıfırlama başlatabilirsiniz.

**Fon şifresi doğru olduğu halde "geçersiz fon şifresi" hatası alıyorum, neden?**
Türkçe şikâyet platformlarında bu başlıkla açılmış onlarca kayıt var. İlk kontrol edilecekler: büyük/küçük harf durumu, klavye dili, tarayıcının otomatik doldurma özelliğinin yanlış şifreyi basması. Sorun devam ederse destek talebi açmak en hızlı yol; ısrarla denemek hesabı gereksiz yere riske atıyor.

**Sıfırladıktan sonra neden 24 saat bekliyorum?**
Hesap güvenlik ayarlarındaki herhangi bir değişiklik çekimleri otomatik olarak 24 saat durduruyor. Bu süre kısaltılamıyor veya destek üzerinden kaldırılamıyor.

**Yalnızca fon şifresi mi bu kilidi tetikliyor?**
Hayır. Giriş şifresi sıfırlama ve 2FA değişiklikleri de aynı 24 saatlik kısıtlamayı başlatıyor.

**Fon şifresi yerine parmak izi veya yüz tanıma kullanabilir miyim?**
Uygulamada biyometrik giriş kolaylık sağlıyor, ancak çekim ve kritik işlem onaylarında fon şifresi istemeye devam ediyor. Biyometrik doğrulama fon şifresinin yerine geçmiyor.

**Fon şifresi ile giriş şifresi aynı olabilir mi?**
Olamaz. Sistem benzer şifreleri de reddediyor, bu yüzden ikisi arasında belirgin bir fark bırakın.

## Kısa özet

Fon şifresi Gate hesabınızda paranın çıkış kapısına takılan ikinci kilit. Belirlemesi üç dakika, unutulduğunda sıfırlaması da yine birkaç dakika — asıl zaman kaybı, sıfırlama sonrası gelen ve kaldırılamayan 24 saatlik çekim kilidi. Hesabınızı yeni açıyorsanız fon şifresini 2FA ile birlikte ilk günden kurun, giriş sıklığını işlem alışkanlığınıza göre seçin ve şifreyi giriş şifresinden net biçimde farklı tutun. Kurulumu şimdi yapmak isterseniz 👉 [Gate kayıt sayfasından](https://bit.ly/GateVIP) hesabınızı açıp güvenlik ayarlarını birkaç dakikada tamamlayabilirsiniz.
