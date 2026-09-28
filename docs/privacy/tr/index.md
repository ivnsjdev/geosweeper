# GeoSweeper için Gizlilik Politikası

**Geçerlilik tarihi:** 26 Eylül 2026

**Son güncelleme:** 26 Eylül 2026

## Kısa versiyon

GeoSweeper hiçbir kişisel bilgiyi toplamaz, iletmez, satmaz veya paylaşmaz. Oynadığınız her tahta, seçtiğiniz her ayar ve temizlediğiniz her ülke yalnızca cihazınızda depolanır. Bize hiçbir şey yüklenmez ve ilk etapta oluşturulacak bir hesap yoktur. GeoSweeper'in şimdiye kadar ürettiği tek ağ trafiği, bir satın alma işlemi yaptığınızda veya geri yüklediğinizde StoreKit'in Apple ile konuşmasıdır ve uygulama içindeki bir bağlantıdan (bu site veya Apple'ın kendi yasal sayfaları) kasıtlı olarak açtığınız sayfalardır - her ikisi de aşağıda ele alınmıştır ve hiçbirinde başka hiçbir şey bulunmamaktadır.

## Biz kimiz

GeoSweeper, Ivan Cayabyab tarafından geliştirilmiştir. Bu politika veya uygulamayla ilgili sorular ivnsjdev@gmail.com'e gönderilebilir.

## Uygulama neyi saklıyor ve nerede

Aşağıdaki her şey yalnızca cihazınızda üç yerden birinde bulunur: "UserDefaults" (küçük ayar değerleri), uygulamanın kendi Uygulama Desteği klasöründeki bir JSON dosyası veya yerel bir SQLite veritabanı.

| Ne | Birincil depolama | Bize otomatik olarak mı gönderildi? |
|---|---|---|
| Ekran ayarları — pano teması, neon rengi, patlama efekti, patlama sesi, harita projeksiyonu (küresel veya düz), ses ve dokunsal etkiyi açma/kapama | 'Kullanıcı Varsayılanları' | Hayır |
| Uygulamanın içinde seçtiğiniz Language | 'Kullanıcı Varsayılanları' | Hayır |
| Derecelendirme istemli defter tutma — GeoSweeper'in iOS'tan yerel derecelendirme tablosunu göstermesini istediği tarihler ve sonuncuyu hangi dönüm noktasının tetiklediği | 'Kullanıcı Varsayılanları' | Hayır |
| Ülke bazında rekor — oynadığınız her ülke için galibiyetler, mağlubiyetler, en iyi zaman ve kilidi açtığınızda | Uygulamanın Uygulama Desteği klasöründeki bir JSON dosyası (`progress.json`) | Hayır |
| Infinite Tower ilerleme — ulaştığınız satır, kayıtlı görünüm pencereniz ve hangi satırları temizlediğiniz | Yerel bir SQLite veritabanı | Hayır |

Bunların hiçbiri biz dahil hiç kimseye iletilmez, satılmaz veya paylaşılmaz. StoreKit'in kendi trafiği (aşağıda) ve dokunduğunuz harici bağlantılar (yine aşağıda) bunların hiçbirini taşımamaktadır. Bir iOS cihazı yedeklemesi, uygulamanın bir bütün olarak yedeklenmesinin bir parçası olarak bu dosyaları içerebilir; bu yedekleme sizin tarafınızdan veya iOS tarafından başlatılır, asla GeoSweeper tarafından başlatılmaz ve bizde değil, gönderdiğiniz yerde (iCloud veya bilgisayarınız) kalır.

## Hesap yok, oturum açma yok, bulut yok

GeoSweeper hiçbir zaman isim, e-posta adresi, telefon numarası, doğum tarihi veya başka herhangi bir tanımlayıcı bilgi istemez; hesap olmadığı için oturum açacak hiçbir şey yoktur. İlerlemeniz iCloud, CloudKit veya başka herhangi bir hizmet aracılığıyla senkronize edilmez: yalnızca oynadığınız cihazda görüntülenir. Aynı ülkeyi ikinci bir cihazda oynayın ve orada yeniden başlayın, çünkü senkronize edilecek hiçbir yerde sunucu kopyası yoktur.

## Kasıtlı olarak ısrar edilmeyen herhangi bir şey

Ortasında olduğunuz tahta, açtığınız her taş, yerleştirdiğiniz her bayrak, yalnızca siz oynarken hafızanızda tutulur. Oyunun ortasında uygulamayı kapattığınızda tahta kaybolur; hiçbir zaman diske yazılmaz ve tamamlanmamış bir panoyu devam ettirmek için otomatik kaydetme yoktur. Yalnızca *bitmiş* bir oyun (galibiyet veya mağlubiyet), yukarıda açıklanan ülke bazında rekoru günceller.

## Yerel değilmiş gibi görünen tek şey

Uygulamayı ilk başlattığınızda harita kendi ülkenizde açılır. Bu, GPS'ten, Wi-Fi'den veya başka herhangi bir konum izleme biçiminden değil, cihazınızın **bölge ayarından** (dilinize ve yerel ayarınıza bağlı ülke; iOS'un klavye ve takvim seçmek için kullandığı ayarın aynısı) gelir. GeoSweeper konum erişimi talep etmiyor ve istese bile koordinatlarınızı okuyamıyor.

## İzinler

GeoSweeper hiçbir şekilde sistem izni istemez. Hiçbir zaman kamerayı, fotoğraf kütüphanesini, mikrofonu, konumu, kişileri, takvimi, sağlık verilerini, hareket verilerini veya anlık bildirimleri istemez ve herhangi bir izin istemi asla görünmez. Bu, uygulamanın "Info.plist"iyle tam olarak eşleşir: İçinde tek bir kullanım açıklaması girişi yoktur.

## Satın Alma İşlemleri

GeoSweeper'i indirmek ücretsizdir. İlk 10 ülkenizi (Beginner dahil herhangi bir seviye) oynamak ücretsizdir ve bir ülkeyi bir kez oynadığınızda, bu ücretsiz deneme bittikten sonra bile tekrar oynanabilir durumda kalır. Infinite Tower, 10. sıraya kadar ücretsizdir. Bu iki noktanın ötesinde, her ikisi de tek seferlik, sarf malzemesi olmayan ve Apple'ın StoreKit'i aracılığıyla sunulan ve tamamen Apple tarafından işlenen iki bağımsız satın alma işlemi vardır:

- **All Countries** — kalıcı olarak kilidi açan tek seferlik, tüketilmeyen bir satın alma işlemidir.
  204 ülkenin tamamında Intermediate, Expert ve Mega katmanları. Bu konuda yenilenen hiçbir şey yok.
- **Infinite Tower Lifetime** — kilidi kalıcı olarak açan, tek seferlik, tüketilmeyen bir satın alma
  10. sırayı geçerek tırmanıyor. Bu konuda da hiçbir şey yenilenmiyor ve GeoSweeper herhangi bir abonelik sunmuyor.

Her ödemeyi GeoSweeper değil Apple gerçekleştirir. Hiçbir kart numarası, fatura adresi veya Apple Account kimlik bilgisi hiçbir zaman tarafımıza görünmez; StoreKit, uygulamaya yalnızca bir ödeme duvarı göstermesi ve erişim izni vermesi için neye ihtiyaç duyduğunu söyler: görüntülenecek fiyat ve her bir öğeye şu anda sahip olup olmadığınız. Bu yanıtlar cihazınızda kalır; GeoSweeper kendi satın alma sunucusunu çalıştırmıyor ve bunları gönderecek hiçbir yeri yok. Satın alınanların geri yüklenmesi, Apple'ın Apple Account cihazınızın neye sahip olduğunu yeniden onaylamasını ister ve yanıtı yerel olarak uygular; herhangi bir yeni kayıt oluşturmaz veya iletmez.

Ayrıca satın alma işlemini yöneten Apple'ın [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) ve [Standart EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/) hükümlerine de bakın.

## İletişimi destekleyin

ivnsjdev@gmail.com'e e-posta gönderirseniz e-posta adresinizi, yazdıklarınızı ve eklemeyi seçtiğiniz ekleri alırız. Bunu yalnızca size yanıt vermek ve hakkında yazdığınız sorunu çözmek için kullanıyoruz; yasal dayanağımız, bizimle iletişime geçen kişilere yanıt verme konusundaki meşru menfaatimizdir. Bu posta kutusu, Google LLC tarafından [Google'ın Gizlilik Politikası](https://policies.google.com/privacy) uyarınca işlenen ve kendi ülkenizin dışında bulunabilecek bir altyapıda barındırılan standart bir Gmail hesabıdır; bu nedenle, söz konusu aktarım burada açıklanmaktadır. Destek e-postalarını 24 aya kadar saklıyoruz ve ardından siliyoruz; İstediğiniz zaman aynı adrese yazarak belirli bir e-postayı daha erken silmemizi isteyebilirsiniz.

## Dış bağlantılar

GeoSweeper'in ödeme duvarları bu sitenin kendi gizlilik politikasına ve Apple'ın Standart EULA'sına bağlantı verir; Settings, App Store'in inceleme yaz sayfasına bağlantı verebilir. Bu bağlantıların hiçbirine hiçbir kullanıcı verisi veya uygulamaya özel tanımlayıcı eklenmez; bunlar herkes için aynı olan düz URL'lerdir.

## Bahse girecek bir şey yok

GeoSweeper'te uygulama içi para birimi, ganimet, ödül çekilişi ve bir sonucun bahise konulduğu veya bahis oynandığı bir özellik yoktur. Her satın alma, içeriğe kalıcı veya zaman sınırlamalı erişim için sabit, açıklanan bir fiyattır; hiçbir şey kazanılamaz, kaybedilemez veya kumar oynanamaz.

## Ne yapmıyoruz

- Hiçbir analitik, kilitlenme raporu veya telemetri yok
- Reklam yok, reklam ağı yok ve reklam tanımlayıcı yok
- Uygulamalar arası veya siteler arası izleme yok ve veri aracıları yok
- Hesap yok, oturum açma yok, şifre yok
- Kamera, fotoğraf kitaplığı, mikrofon, kişiler, kesin veya kaba konum veya sağlık verileri yok
- Verileriniz üzerinde makine öğrenimi modelleri eğitimi yok
- Hiçbir türde üçüncü taraf SDK yok — bu uygulamadaki tek kod bize aittir

Bu, GeoSweeper'in App Store üzerinde taşıdığı "Data Not Collected (veri toplanmıyor)" etiketiyle eşleşir.

## Saklama ve silme

Uygulamanın silinmesi, cihazınızda depolanan her dosyayı (ayarlar, ülke başına kaydınız ve Infinite Tower ilerlemeniz) anında ve tamamen siler, çünkü bizim tarafımızdan tutulacak veya silinecek bir sunucu kopyası hiçbir zaman olmadı. Silme işleminden önce oluşturulan bir iCloud cihazı yedeklemesi hâlâ bir kopya içerebilir; Bu yedekleme, cihazınızdaki **Settings → adınız → iCloud → Hesap Depolama Alanını Yönet** yoluyla tamamen sizin kontrolünüz altındadır. Destek e-postaları yukarıda açıklandığı gibi ayrı olarak saklanır ve silinir.

## Haklarınız

GeoSweeper, uygulama içi verilerinizin hiçbir kopyasını saklamadığından, GDPR, Birleşik Krallık GDPR ve CCPA/CPRA'nın tanımladığı erişim, düzeltme, dışa aktarma ve silme hakları, halihazırda kendi cihazınızda doğrudan kullandığınız haklardır; burada sizin adınıza oluşturabileceğimiz veya silebileceğimiz bir kayıt yoktur. Bir şeyi sakladığımız tek yer, bize gönderdiğiniz destek e-postasıdır ve istediğiniz zaman ivnsjdev@gmail.com'e yazarak bunu görmeyi, düzeltmeyi veya silmeyi isteyebilirsiniz. Bağlamlar arası davranışsal reklamcılık için kişisel bilgileri satmıyor veya paylaşmıyoruz ve asla paylaşmayacağız. Verilerinizi yanlış kullandığımızı düşünüyorsanız yerel veri koruma yetkilinize şikayette bulunma hakkına sahipsiniz.

## Çocuklar

GeoSweeper, genel izleyici kitlesine uygun bir yaş derecelendirmesine sahiptir ve özellikle çocuklara yönelik değildir. 13 yaşın altındaki çocuklar da dahil olmak üzere hiç kimseden bilerek kişisel bilgi toplamıyoruz ve uygulamada bunu yapabilecek hiçbir şey yok: sohbet yok, paylaşım yok, sosyal özellik yok, reklam yok ve bir çocuğa ulaşmak için üçüncü bir tarafın hesabı yok.

## Bu politikada yapılan değişiklikler

Bu politika değişirse üstteki tarih de onunla birlikte değişecek ve GeoSweeper'in verilerle yaptığı önemli değişiklik de bu güncellemenin sürüm notlarında belirtilecektir.

## İletişim

ivnsjdev@gmail.com
