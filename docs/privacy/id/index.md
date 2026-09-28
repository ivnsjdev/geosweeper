# Kebijakan Privasi untuk GeoSweeper

**Tanggal efektif:** 26 September 2026

**Terakhir diperbarui:** 26 September 2026

## Versi pendek

GeoSweeper tidak mengumpulkan, mengirimkan, menjual, atau membagikan informasi pribadi apa pun. Setiap papan yang Anda mainkan, setiap pengaturan yang Anda pilih, dan setiap negara yang Anda selesaikan hanya disimpan di perangkat Anda. Tidak ada yang diunggah ke kami, dan tidak ada akun yang harus dibuat. Satu-satunya lalu lintas jaringan yang pernah dihasilkan GeoSweeper adalah StoreKit berbicara dengan Apple saat Anda melakukan atau memulihkan pembelian, dan halaman yang sengaja Anda buka dari tautan di dalam aplikasi (situs ini, atau halaman resmi Apple sendiri) — keduanya tercakup di bawah, dan tidak ada yang membawa hal lain di dalamnya.

## Siapa kita

GeoSweeper dikembangkan oleh Ivan Cayabyab. Pertanyaan tentang kebijakan ini atau aplikasi dapat dikirim ke ivnsjdev@gmail.com.

## Apa yang disimpan aplikasinya, dan di mana

Segala sesuatu di bawah hanya ada di perangkat Anda, di salah satu dari tiga tempat: `UserDefaults` (nilai pengaturan kecil), file JSON di folder Dukungan Aplikasi milik aplikasi, atau database SQLite lokal.

| Apa | Penyimpanan utama | Dikirim secara otomatis kepada kami? |
|---|---|---|
| Pengaturan tampilan — tema papan, warna neon, efek ledakan, suara ledakan, proyeksi peta (bola dunia atau datar), suara dan haptik aktif/nonaktif | `Default Pengguna` | Tidak |
| Language yang Anda pilih di dalam aplikasi | `Default Pengguna` | Tidak |
| Pembukuan berdasarkan peringkat — tanggal GeoSweeper meminta iOS untuk menampilkan lembar peringkat asli, dan pencapaian mana yang memicu lembar peringkat terakhir | `Default Pengguna` | Tidak |
| Rekor per negara — kemenangan, kekalahan, waktu terbaik, dan kapan Anda membukanya, untuk setiap negara yang Anda mainkan | File JSON (`progress.json`) di folder Dukungan Aplikasi aplikasi | Tidak |
| Kemajuan Infinite Tower — baris yang telah Anda capai, area pandang yang disimpan, dan baris mana yang telah Anda kosongkan | Basis data SQLite lokal | Tidak |

Semua ini tidak disebarkan, dijual, atau dibagikan kepada siapa pun, termasuk kami. Lalu lintas StoreKit sendiri (di bawah) dan tautan eksternal yang Anda ketuk (juga di bawah) tidak membawa apa pun. Pencadangan perangkat iOS dapat menyertakan file-file ini sebagai bagian dari pencadangan aplikasi secara keseluruhan — pencadangan tersebut dimulai oleh Anda atau oleh iOS, tidak pernah oleh GeoSweeper, dan cadangan tersebut tetap ada di mana pun Anda mengirimkannya (iCloud atau komputer Anda), bukan pada kami.

## Tanpa akun, tanpa masuk, tanpa cloud

GeoSweeper tidak pernah menanyakan nama, alamat email, nomor telepon, tanggal lahir, atau informasi identitas lainnya — tidak ada yang perlu digunakan untuk masuk, karena tidak ada akun. Kemajuan Anda tidak disinkronkan melalui iCloud, CloudKit, atau layanan lainnya: kemajuan hanya ada di perangkat yang Anda gunakan untuk bermain. Mainkan negara yang sama di perangkat kedua dan itu akan dimulai dari sana, karena tidak ada salinan server di mana pun untuk disinkronkan.

## Apa pun yang sengaja tidak dipertahankan

Papan tempat Anda berada — setiap ubin yang Anda buka, setiap bendera yang Anda tempatkan — hanya disimpan dalam memori saat Anda bermain. Tutup aplikasi di tengah permainan dan papan itu hilang; itu tidak pernah ditulis ke disk, dan tidak ada penyimpanan otomatis untuk melanjutkan papan yang belum selesai. Hanya permainan *selesai* (menang atau kalah) yang memperbarui rekor per negara yang dijelaskan di atas.

## Satu hal yang sepertinya bukan hal lokal

Peta akan terbuka di negara Anda saat pertama kali Anda meluncurkan aplikasi. Ini berasal dari **setelan wilayah** perangkat Anda (negara yang terkait dengan bahasa dan lokal Anda, sama dengan yang digunakan iOS untuk memilih keyboard dan kalender) — bukan dari GPS, Wi-Fi, atau bentuk pelacakan lokasi lainnya. GeoSweeper tidak meminta akses lokasi dan tidak dapat membaca koordinat Anda meskipun ia menginginkannya.

## Izin

GeoSweeper tidak meminta izin sistem apa pun. Itu tidak pernah meminta kamera, perpustakaan foto, mikrofon, lokasi, kontak, kalender, data kesehatan, data gerakan, atau pemberitahuan push, dan tidak ada permintaan izin apa pun yang akan muncul. Ini sama persis dengan `Info.plist` aplikasi: tidak ada satu pun entri deskripsi penggunaan di dalamnya.

## Pembelian

GeoSweeper gratis untuk diunduh. 10 negara pertama Anda — tingkat mana pun, termasuk Beginner — gratis untuk dimainkan, dan setelah Anda memainkan suatu negara, negara tersebut tetap dapat diputar ulang selamanya, bahkan setelah uji coba gratis tersebut habis. Infinite Tower gratis hingga baris 10. Di luar kedua poin tersebut, terdapat dua pembelian independen, keduanya satu kali, tidak dapat dikonsumsi, dan ditawarkan melalui StoreKit Apple dan diproses seluruhnya oleh Apple:

- **All Countries** — pembelian satu kali yang tidak dapat dikonsumsi dan membuka kunci secara permanen
  Tingkat Intermediate, Expert, dan Mega di seluruh 204 negara. Tidak ada yang diperbarui tentang ini.
- **Infinite Tower Lifetime** — pembelian satu kali yang tidak dapat dikonsumsi dan terbuka secara permanen
  memanjat melewati baris 10. Tidak ada pembaruan apa pun tentang ini, dan GeoSweeper tidak menawarkan langganan apa pun.

Apple, bukan GeoSweeper, yang memproses setiap pembayaran. Tidak ada nomor kartu, alamat penagihan, atau kredensial Apple Account yang dapat kami lihat — StoreKit hanya memberi tahu aplikasi apa yang diperlukan untuk menampilkan paywall dan memberikan akses: harga yang akan ditampilkan, dan apakah Anda saat ini memiliki setiap item. Jawaban-jawaban itu tetap ada di perangkat Anda; GeoSweeper tidak menjalankan server pembeliannya sendiri dan tidak memiliki tempat untuk mengirimkannya. Memulihkan pembelian meminta Apple untuk mengonfirmasi ulang apa yang dimiliki Apple Account Anda dan menerapkan jawabannya secara lokal — ini tidak membuat atau mengirimkan rekor baru apa pun.

Lihat juga [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/), dan [Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/) Apple, yang mengatur pembelian itu sendiri.

## Mendukung komunikasi

Jika Anda mengirim email ivnsjdev@gmail.com, kami menerima alamat email Anda, apa pun yang Anda tulis, dan lampiran apa pun yang Anda pilih untuk ditambahkan. Kami menggunakannya hanya untuk menjawab Anda dan memperbaiki masalah yang Anda tulis — dasar hukum kami adalah kepentingan sah kami dalam menanggapi orang yang menghubungi kami. Kotak surat tersebut adalah akun Gmail standar, diproses oleh Google LLC berdasarkan [Kebijakan Privasi Google](https://policies.google.com/privacy), dan dihosting di infrastruktur yang mungkin berlokasi di luar negara Anda, itulah sebabnya transfer tersebut diungkapkan di sini. Kami menyimpan email dukungan hingga 24 bulan dan kemudian menghapusnya; Anda dapat meminta kami untuk menghapus email tertentu lebih cepat kapan saja dengan menulis ke alamat yang sama.

## Tautan eksternal

Tautan paywall GeoSweeper ke kebijakan privasi situs ini dan EULA Standar Apple; Settings dapat menautkan ke halaman tulis ulasan App Store. Tidak ada data pengguna atau pengenal khusus aplikasi yang ditambahkan ke tautan mana pun — ini adalah URL biasa, sama untuk semua orang.

## Tidak ada yang perlu dipertaruhkan

GeoSweeper tidak memiliki mata uang dalam aplikasi, tidak ada jarahan, tidak ada pengundian hadiah, dan tidak ada fitur di mana suatu hasil dipertaruhkan atau dipertaruhkan. Setiap pembelian adalah harga tetap dan diungkapkan untuk akses permanen atau terbatas waktu ke konten; tidak ada yang bisa dimenangkan, dikalahkan, atau dipertaruhkan.

## Apa yang TIDAK kami lakukan

- Tidak ada analitik, pelaporan kerusakan, atau telemetri apa pun
- Tidak ada iklan, tidak ada jaringan iklan, dan tidak ada pengidentifikasi iklan
- Tidak ada pelacakan lintas aplikasi atau lintas situs, dan tidak ada broker data
- Tanpa akun, tanpa login, tanpa kata sandi
- Tidak ada kamera, perpustakaan foto, mikrofon, kontak, lokasi akurat atau kasar, atau data kesehatan
- Tidak ada pelatihan model pembelajaran mesin pada data Anda
- Tidak ada SDK pihak ketiga apa pun — satu-satunya kode di aplikasi ini adalah milik kami sendiri

Ini cocok dengan label "Data Not Collected (data tidak dikumpulkan)" yang dibawa GeoSweeper pada App Store.

## Retensi dan penghapusan

Menghapus aplikasi akan menghapus setiap file yang tersimpan di perangkat Anda — pengaturan, catatan per negara, dan kemajuan Infinite Tower Anda — secara langsung dan menyeluruh, karena tidak pernah ada salinan server yang dapat kami simpan atau hapus di pihak kami. Cadangan perangkat iCloud yang dibuat sebelum penghapusan mungkin masih berisi salinan; pencadangan tersebut sepenuhnya berada di bawah kendali Anda melalui **Settings → nama Anda → iCloud → Kelola Penyimpanan Akun** di perangkat Anda. Email dukungan disimpan dan dihapus secara terpisah, seperti dijelaskan di atas.

## Hak Anda

Karena GeoSweeper tidak menyimpan salinan data dalam aplikasi Anda, hak akses, koreksi, ekspor, dan penghapusan yang dijelaskan oleh GDPR, GDPR Inggris, dan CCPA/CPRA adalah hak yang sudah Anda gunakan secara langsung, di perangkat Anda sendiri — tidak ada catatan di sini untuk kami buat atau hapus atas nama Anda. Satu-satunya tempat kami menyimpan sesuatu adalah email dukungan yang Anda kirimkan kepada kami, dan Anda dapat meminta untuk melihat, memperbaiki, atau menghapusnya kapan saja dengan menulis ke ivnsjdev@gmail.com. Kami tidak menjual atau membagikan informasi pribadi untuk periklanan perilaku lintas konteks, dan tidak pernah melakukannya. Jika Anda yakin kami telah salah menangani data Anda, Anda berhak mengajukan keluhan kepada otoritas perlindungan data setempat.

## Anak-anak

GeoSweeper mengusung rating usia yang cocok untuk khalayak umum dan tidak ditujukan untuk anak-anak secara khusus. Kami tidak dengan sengaja mengumpulkan informasi pribadi dari siapa pun, termasuk anak-anak di bawah 13 tahun, dan tidak ada apa pun di dalam aplikasi yang dapat melakukannya — tidak ada obrolan, tidak ada berbagi, tidak ada fitur sosial, tidak ada iklan, dan tidak ada akun pihak ketiga yang dapat menjangkau anak tersebut.

## Perubahan pada kebijakan ini

Jika kebijakan ini berubah, tanggal di atas juga akan ikut berubah, dan perubahan material terhadap apa yang dilakukan GeoSweeper dengan data juga akan dicatat dalam catatan rilis pembaruan tersebut.

## Kontak

ivnsjdev@gmail.com
