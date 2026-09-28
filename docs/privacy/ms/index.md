# Dasar Privasi untuk GeoSweeper

**Tarikh berkuatkuasa:** 26 September 2026

**Terakhir dikemas kini:** 26 September 2026

## Versi pendek

GeoSweeper tidak mengumpul, menghantar, menjual atau berkongsi sebarang maklumat peribadi. Setiap papan yang anda mainkan, setiap tetapan yang anda pilih dan setiap negara yang telah anda bersihkan disimpan hanya pada peranti anda. Tiada apa-apa yang dimuat naik kepada kami, dan tiada akaun untuk dibuat pada mulanya. Satu-satunya trafik rangkaian GeoSweeper yang pernah dihasilkan ialah StoreKit bercakap dengan Apple apabila anda membuat atau memulihkan pembelian, dan halaman yang anda sengaja buka daripada pautan di dalam apl (tapak ini, atau halaman undang-undang Apple sendiri) — kedua-duanya dilindungi di bawah dan tidak membawa apa-apa lagi bersamanya.

## Siapa kita

GeoSweeper dibangunkan oleh Ivan Cayabyab. Soalan tentang dasar ini atau apl boleh dihantar ke ivnsjdev@gmail.com.

## Perkara yang disimpan oleh apl itu dan di mana

Semua perkara di bawah hanya hidup pada peranti anda, di salah satu daripada tiga tempat: `UserDefaults` (nilai tetapan kecil), fail JSON dalam folder Sokongan Aplikasi apl itu sendiri atau pangkalan data SQLite setempat.

| Apa | Storan utama | Dihantar secara automatik kepada kami? |
|---|---|---|
| Tetapan paparan — tema papan, warna neon, kesan letupan, bunyi letupan, unjuran peta (glob atau rata), bunyi dan haptik hidup/mati | `UserDefaults` | Tidak |
| Language yang telah anda pilih dalam apl | `UserDefaults` | Tidak |
| Simpan kira kadar segera — tarikh GeoSweeper telah meminta iOS untuk menunjukkan helaian penilaian asli, dan peristiwa penting mana yang mencetuskan yang terakhir | `UserDefaults` | Tidak |
| Rekod setiap negara — menang, kalah, masa terbaik dan apabila anda membuka kuncinya, untuk setiap negara yang telah anda mainkan | Fail JSON (`progress.json`) dalam folder Sokongan Aplikasi apl | Tidak |
| Kemajuan Infinite Tower — baris yang telah anda capai, port pandangan anda yang disimpan dan baris mana yang telah anda kosongkan | Pangkalan data SQLite tempatan | Tidak |

Tiada satu pun daripada ini dihantar, dijual atau dikongsi dengan sesiapa sahaja, termasuk kami. Trafik StoreKit sendiri (di bawah) dan pautan luaran yang anda ketik (juga di bawah) tidak membawanya. Sandaran peranti iOS mungkin termasuk fail ini sebagai sebahagian daripada sandaran apl secara keseluruhan — sandaran itu dimulakan oleh anda atau oleh iOS, tidak sekali-kali oleh GeoSweeper, dan ia kekal di mana-mana sahaja anda menghantarnya (iCloud atau komputer anda), bukan dengan kami.

## Tiada akaun, tiada log masuk, tiada awan

GeoSweeper tidak pernah meminta nama, alamat e-mel, nombor telefon, tarikh lahir atau sebarang maklumat pengenalan lain — tiada apa-apa untuk log masuk, kerana tiada akaun. Kemajuan anda tidak disegerakkan melalui iCloud, CloudKit atau mana-mana perkhidmatan lain: ia hanya hidup pada peranti yang anda mainkan. Mainkan negara yang sama pada peranti kedua dan ia bermula baharu di sana, kerana tiada salinan pelayan di mana-mana untuk disegerakkan.

## Apa-apa pun sengaja tidak berterusan

Papan yang anda berada di tengah-tengah — setiap jubin yang anda buka, setiap bendera yang anda letakkan — hanya disimpan dalam ingatan semasa anda bermain. Tutup apl pada pertengahan permainan dan papan itu hilang; ia tidak pernah ditulis pada cakera, dan tiada autosimpan untuk menyambung semula papan yang belum selesai. Hanya permainan *selesai* (menang atau kalah) mengemas kini rekod setiap negara yang diterangkan di atas.

## Satu perkara yang kelihatan seperti ia bukan tempatan

Peta dibuka di negara anda sendiri pada kali pertama anda melancarkan apl. Ini datang daripada **tetapan wilayah** peranti anda (negara yang terikat dengan bahasa dan tempat anda, yang sama digunakan oleh iOS untuk memilih papan kekunci dan kalendar) — bukan daripada GPS, Wi-Fi atau sebarang bentuk penjejakan lokasi lain. GeoSweeper tidak meminta akses lokasi dan tidak dapat membaca koordinat anda walaupun ia mahu.

## Kebenaran

GeoSweeper tidak meminta kebenaran sistem sama sekali. Ia tidak pernah meminta kamera, pustaka foto, mikrofon, lokasi, kenalan, kalendar, data kesihatan, data gerakan atau pemberitahuan tolak, dan sebarang jenis gesaan kebenaran tidak akan muncul. Ini sepadan dengan `Info.plist` apl dengan tepat: tiada satu pun entri perihalan penggunaan di dalamnya.

## Pembelian

GeoSweeper adalah percuma untuk dimuat turun. 10 negara pertama anda — mana-mana peringkat, termasuk Beginner — adalah percuma untuk dimainkan dan sebaik sahaja anda bermain sesebuah negara, negara itu kekal boleh dimainkan semula untuk selama-lamanya, walaupun selepas percubaan percuma itu dibelanjakan. Infinite Tower adalah percuma sehingga baris 10. Di sebalik dua mata itu, terdapat dua pembelian bebas, kedua-duanya sekali, tidak boleh habis, dan ditawarkan melalui StoreKit Apple dan diproses sepenuhnya oleh Apple:

- **All Countries** — pembelian sekali sahaja, tidak boleh habis yang membuka kunci secara kekal
  Peringkat Intermediate, Expert dan Mega merentas semua 204 negara. Tiada apa-apa tentang ini diperbaharui.
- **Infinite Tower Lifetime** — pembelian sekali sahaja, tidak boleh habis yang membuka kunci secara kekal
  mendaki melepasi baris 10. Tiada apa-apa tentang ini diperbaharui sama ada, dan GeoSweeper tidak menawarkan sebarang jenis langganan.

Apple, bukan GeoSweeper, memproses setiap pembayaran. Tiada nombor kad, alamat pengebilan atau bukti kelayakan Apple Account pernah kelihatan kepada kami — StoreKit hanya memberitahu apl perkara yang diperlukan untuk menunjukkan tembok berbayar dan memberikan akses: harga untuk dipaparkan dan sama ada anda memiliki setiap item pada masa ini. Jawapan tersebut kekal pada peranti anda; GeoSweeper tidak menjalankan pelayan pembelian sendiri dan tidak mempunyai tempat untuk menghantarnya. Memulihkan pembelian meminta Apple mengesahkan semula perkara yang dimiliki oleh Apple Account anda dan menggunakan jawapan secara setempat — ia tidak mencipta atau menghantar sebarang rekod baharu.

Lihat juga [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/) Apple, [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) dan [EULA Standard](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), yang mengawal pembelian itu sendiri.

## Menyokong komunikasi

Jika anda menghantar e-mel kepada ivnsjdev@gmail.com, kami menerima alamat e-mel anda, apa sahaja yang anda tulis dan sebarang lampiran yang anda pilih untuk ditambah. Kami menggunakannya hanya untuk menjawab anda dan untuk menyelesaikan masalah yang anda tulis tentang — asas sah kami ialah kepentingan sah kami untuk membalas orang yang menghubungi kami. Peti mel itu ialah akaun Gmail standard, diproses oleh Google LLC di bawah [Dasar Privasi Google](https://policies.google.com/privacy) dan dihoskan pada infrastruktur yang mungkin terletak di luar negara anda sendiri, itulah sebabnya pemindahan itu didedahkan di sini. Kami menyimpan e-mel sokongan sehingga 24 bulan dan kemudian memadamkannya; anda boleh meminta kami memadamkan e-mel tertentu lebih awal pada bila-bila masa dengan menulis ke alamat yang sama.

## Pautan luar

Paywall GeoSweeper memaut ke dasar privasi tapak ini sendiri dan ke EULA Standard Apple; Settings boleh memaut ke halaman tulis-semakan App Store. Tiada data pengguna atau pengecam khusus apl dilampirkan pada mana-mana pautan ini — ia adalah URL biasa, sama untuk semua orang.

## Tiada apa untuk dipertaruhkan

GeoSweeper tidak mempunyai mata wang dalam apl, tiada rampasan, tiada cabutan hadiah dan tiada ciri di mana keputusan dipertaruhkan atau dipertaruhkan. Setiap pembelian ialah harga tetap yang didedahkan untuk akses kekal atau berkotak masa kepada kandungan; tiada apa yang boleh dimenangi, kalah atau diperjudikan.

## Apa yang TIDAK kami lakukan

- Tiada analitik, pelaporan ranap atau telemetri dalam apa jua bentuk
- Tiada pengiklanan, tiada rangkaian iklan dan tiada pengecam pengiklanan
- Tiada penjejakan merentas apl atau merentas tapak, dan tiada broker data
- Tiada akaun, tiada log masuk, tiada kata laluan
- Tiada kamera, pustaka foto, mikrofon, kenalan, lokasi tepat atau kasar, atau data kesihatan
- Tiada latihan model pembelajaran mesin pada data anda
- Tiada jenis SDK pihak ketiga — satu-satunya kod dalam apl ini adalah milik kami

Ini sepadan dengan label "Data Not Collected (data tidak dikumpul)" GeoSweeper yang dibawa pada App Store.

## Pengekalan dan pemadaman

Memadamkan apl memadamkan setiap fail yang disimpan pada peranti anda — tetapan, rekod setiap negara anda dan kemajuan Infinite Tower anda — serta-merta dan sepenuhnya, kerana tidak pernah ada salinan pelayan untuk kami pegang atau dipadamkan di pihak kami. Sandaran peranti iCloud yang dibuat sebelum pemadaman mungkin masih mengandungi salinan; sandaran itu berada di bawah kawalan anda sepenuhnya melalui **Settings → nama anda → iCloud → Urus Storan Akaun** pada peranti anda. E-mel sokongan disimpan dan dipadam secara berasingan, seperti yang diterangkan di atas.

## Hak anda

Oleh kerana GeoSweeper tidak menyimpan sebarang salinan data dalam apl anda, hak akses, pembetulan, eksport dan pemadaman yang digambarkan oleh GDPR, GDPR UK dan CCPA/CPRA adalah hak yang anda sudah gunakan secara langsung, pada peranti anda sendiri — tiada rekod di sini untuk kami hasilkan atau padamkan bagi pihak anda. Satu-satunya tempat kami memegang sesuatu ialah e-mel sokongan yang telah anda hantar kepada kami dan anda boleh meminta untuk melihat, membetulkan atau memadamkannya pada bila-bila masa dengan menulis kepada ivnsjdev@gmail.com. Kami tidak menjual atau berkongsi maklumat peribadi untuk pengiklanan tingkah laku merentas konteks, dan tidak pernah melakukannya. Jika anda percaya kami telah salah mengendalikan data anda, anda mempunyai hak untuk membuat aduan kepada pihak berkuasa perlindungan data tempatan anda.

## Kanak-kanak

GeoSweeper membawa penilaian umur yang sesuai untuk khalayak umum dan tidak ditujukan kepada kanak-kanak secara khusus. Kami tidak sengaja mengumpul maklumat peribadi daripada sesiapa, termasuk kanak-kanak bawah 13 tahun, dan tiada apa-apa dalam apl yang boleh — tiada sembang, tiada perkongsian, tiada ciri sosial, tiada pengiklanan dan tiada akaun untuk pihak ketiga untuk menghubungi kanak-kanak melalui.

## Perubahan kepada dasar ini

Jika dasar ini berubah, tarikh di bahagian atas akan berubah bersamanya dan perubahan penting kepada perkara yang GeoSweeper lakukan dengan data juga akan dicatatkan dalam nota keluaran kemas kini itu.

## Hubungi

ivnsjdev@gmail.com
