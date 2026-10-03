# Google Indexing Audit & Technical SEO

## Gambaran Proyek

Proyek ini merupakan dokumentasi portofolio pekerjaan **Technical SEO** yang berfokus pada audit status pengindeksan website melalui **Google Search Console**.

Audit dilakukan untuk mengidentifikasi URL yang mengalami kendala pada proses crawling dan indexing, mengklasifikasikan setiap isu berdasarkan status yang terdeteksi, serta menyusun rekomendasi teknis yang dapat ditindaklanjuti oleh pihak terkait.

Proses analisis mencakup pemeriksaan berbagai status URL, seperti **Not Found (404)**, **Page with Redirect**, **Redirect Error**, **Crawled – Currently Not Indexed**, **Excluded by `noindex` Tag**, dan **Blocked by robots.txt**. Hasil audit kemudian didokumentasikan dalam spreadsheet sebagai acuan untuk proses review, implementasi, dan monitoring perbaikan.

> **Catatan:** Nama klien, domain, URL, data bisnis, serta informasi internal telah dianonimkan atau dihapus untuk keperluan portofolio.

---

## Tujuan Proyek

- Mengidentifikasi URL yang mengalami masalah crawling atau indexing
- Menganalisis status URL berdasarkan laporan Google Search Console
- Mengelompokkan isu berdasarkan jenis permasalahan teknis
- Menentukan prioritas URL yang memerlukan tindak lanjut
- Menyusun rekomendasi terkait redirect, crawlability, dan indexability
- Mendokumentasikan hasil audit untuk memudahkan proses implementasi
- Mendukung monitoring status indexing setelah perbaikan diterapkan

---

## Alur Audit

```text
Google Search Console
        ↓
Ekspor Laporan Indexing
        ↓
Klasifikasi URL dan Status
        ↓
Analisis Isu Teknis
        ↓
Penyusunan Rekomendasi
        ↓
Review PM / Stakeholder
        ↓
Persetujuan Klien
        ↓
Implementasi oleh Tim Development
        ↓
Monitoring dan Tindak Lanjut
```

---

## Status Indexing yang Dianalisis

| Status | Fokus Analisis |
|---|---|
| Not Found (404) | Mengidentifikasi halaman yang tidak ditemukan dan menentukan apakah URL perlu dipertahankan, dialihkan, atau dibiarkan menghasilkan status 404 |
| Page with Redirect | Memeriksa URL yang mengarah ke halaman lain serta memastikan tujuan redirect relevan dan berfungsi dengan benar |
| Redirect Error | Mengidentifikasi masalah pada proses redirect, seperti redirect loop, rantai redirect, atau URL tujuan yang tidak dapat diakses |
| Crawled – Currently Not Indexed | Meninjau halaman yang telah dirayapi Google tetapi belum dipilih untuk masuk ke indeks |
| Excluded by `noindex` Tag | Memastikan penggunaan tag `noindex` sudah sesuai dengan tujuan pengelolaan halaman |
| Blocked by robots.txt | Mengidentifikasi URL yang tidak dapat dirayapi karena aturan dalam file `robots.txt` |
| Blocked due to Access Forbidden | Meninjau URL yang tidak dapat diakses oleh Googlebot karena pembatasan akses server atau konfigurasi keamanan |
| Indexed Pages | Memastikan halaman penting yang seharusnya tampil di hasil pencarian telah berhasil diindeks |

---

## Data yang Dianalisis

| Data | Tujuan Analisis |
|---|---|
| URL | Mengidentifikasi halaman yang mengalami isu teknis |
| Indexing Status | Menentukan status URL berdasarkan laporan Google Search Console |
| Last Crawl | Mengetahui waktu terakhir Google melakukan crawling pada URL |
| URL Type | Mengelompokkan URL berdasarkan jenis halaman, seperti produk, kategori, artikel, filter, atau parameter |
| SEO / Technical Notes | Mendokumentasikan hasil pemeriksaan dan konteks setiap isu |
| Recommended Action | Menentukan tindakan teknis yang direkomendasikan |
| Implementation Status | Melacak progres implementasi rekomendasi |
| Follow-up Notes | Mencatat kebutuhan review, approval, atau tindak lanjut dari PM dan tim development |

---

## Dokumentasi Proyek

| Tahap | Deskripsi | Dokumentasi |
|---|---|---|
| **Task / Project Brief** | **project brief untuk Google Indexing Audit**, termasuk tujuan audit, kondisi yang menjadi prasyarat pengerjaan, serta instruksi untuk meninjau laporan Google Search Console.
Task berfokus pada identifikasi masalah crawling dan indexing, dokumentasi URL yang membutuhkan tindakan, serta penyusunan rekomendasi untuk ditinjau oleh Project Manager dan tim terkait. | <img src="assets/screenshots/google%20indexing%201.PNG" alt="Task brief Google Indexing Audit" width="500"> |
| **Indexing Report** | Laporan Google Search Console digunakan untuk mengelompokkan URL berdasarkan status indexing dan menentukan halaman yang memerlukan pemeriksaan lebih lanjut. | <img src="assets/screenshots/google%20indexing%202.PNG" alt="Google Search Console indexing report" width="500"> |
| **Klasifikasi Status URL** | URL dikelompokkan berdasarkan jenis isu, seperti 404, redirect, halaman yang telah di-crawl tetapi belum diindeks, `noindex`, dan pembatasan crawling. | <img src="assets/screenshots/google%20indexing%203.PNG" alt="Klasifikasi status indexing URL" width="500"> |
| **Analisis dan Rekomendasi** | Setiap URL dianalisis berdasarkan status, jenis halaman, internal linking, serta tindakan yang disarankan, termasuk redirect, perbaikan teknis, atau monitoring lanjutan. | <img src="assets/screenshots/google%20indexing%204.PNG" alt="Analisis URL dan rekomendasi Technical SEO" width="500"> |
| **Implementation Follow-up** | Hasil audit didokumentasikan untuk proses review bersama PM, persetujuan stakeholder, implementasi oleh tim development, serta tindak lanjut setelah perbaikan diterapkan. | <img src="assets/screenshots/google%20indexing%205.PNG" alt="Tindak lanjut implementasi Google Indexing Audit" width="500"> |

---

## Contoh Temuan

### URL dengan Status 404

Salah satu kelompok URL yang ditemukan dalam audit adalah halaman produk dengan status **Not Found (404)**.

Berdasarkan pemeriksaan, sebagian URL merupakan halaman produk yang sudah tidak tersedia. Tindakan yang direkomendasikan ditentukan berdasarkan relevansi URL, ketersediaan halaman pengganti, nilai traffic, backlink, serta kebutuhan bisnis.

| Kondisi URL | Rekomendasi Potensial |
|---|---|
| Produk tidak tersedia sementara | Mempertahankan URL apabila produk berpotensi tersedia kembali dan memastikan halaman 404 memberikan navigasi yang membantu pengguna |
| Produk dihentikan secara permanen | Mempertimbangkan redirect 301 ke halaman kategori, produk alternatif, atau halaman pengganti yang paling relevan |
| Tidak tersedia halaman pengganti yang relevan | Mempertahankan status 404 atau 410, terutama apabila URL tidak memiliki nilai SEO, traffic, maupun backlink yang signifikan |
| URL masih menerima internal link | Memperbarui atau menghapus internal link yang mengarah ke URL 404 |

Redirect tidak direkomendasikan secara otomatis untuk seluruh halaman 404. Redirect hanya dipertimbangkan apabila terdapat halaman tujuan yang relevan bagi pengguna dan sesuai dengan konteks halaman sebelumnya.

### URL dengan Parameter Dinamis

Audit juga menemukan URL dengan parameter dinamis, misalnya:

```text
?pr_prod
```

URL tersebut diidentifikasi sebagai parameter yang digunakan untuk menghasilkan rekomendasi produk secara dinamis. Pemeriksaan dilakukan untuk mengetahui apakah parameter tersebut:

- Memiliki nilai SEO atau traffic organik
- Menjadi target internal link yang penting
- Menghasilkan konten duplikat atau variasi URL yang tidak diperlukan
- Perlu dapat di-crawl oleh Google
- Memerlukan canonicalisasi, pengaturan parameter, atau pembatasan crawling

Apabila URL parameter tidak memberikan nilai SEO dan berpotensi menghabiskan crawl budget, rekomendasi dapat mencakup perbaikan internal linking, penggunaan canonical yang sesuai, atau pembatasan crawling melalui `robots.txt` setelah dilakukan validasi teknis.

> **Catatan teknis:** `robots.txt` digunakan untuk mengatur crawling, bukan untuk memastikan sebuah URL dihapus dari indeks. Jika sebuah halaman perlu dikeluarkan dari hasil pencarian, pendekatan yang lebih sesuai dapat berupa tag `noindex` pada halaman yang tetap dapat di-crawl, penghapusan URL, redirect ke halaman relevan, atau penggunaan alat penghapusan sementara di Google Search Console sesuai kebutuhan.

---

## Rekomendasi yang Dihasilkan

Berdasarkan hasil audit, rekomendasi teknis yang dapat diberikan meliputi:

- Menambahkan redirect 301 untuk halaman yang telah dipindahkan atau dihapus dan memiliki halaman pengganti yang relevan
- Mengarahkan URL lama ke halaman pengganti yang paling sesuai bagi pengguna
- Memperbaiki redirect error, redirect loop, atau rantai redirect yang tidak diperlukan
- Meninjau konfigurasi teknis yang memengaruhi kemampuan Googlebot untuk melakukan crawling
- Mengevaluasi aturan dalam file `robots.txt`
- Meninjau penggunaan tag `noindex` untuk memastikan penerapannya sesuai tujuan
- Memeriksa dan memperbarui internal link yang mengarah ke URL bermasalah
- Mengevaluasi halaman berstatus *Crawled – Currently Not Indexed* dari sisi kualitas, duplikasi, canonical, dan nilai konten
- Memastikan halaman penting tersedia dalam XML sitemap dan dapat diakses oleh crawler
- Melakukan monitoring status indexing setelah implementasi perbaikan

---

## Kolaborasi dan Alur Kerja

Audit Technical SEO melibatkan koordinasi dengan beberapa pihak agar rekomendasi yang disusun dapat diimplementasikan secara tepat dan sesuai dengan kebutuhan bisnis.

```text
SEO / Inbound Marketing
        ↓
Review Project Manager
        ↓
Persetujuan Klien / Stakeholder
        ↓
Tim Frontend atau Development
        ↓
Review Implementasi
        ↓
Monitoring dan Tindak Lanjut
```

Beberapa rekomendasi teknis memerlukan persetujuan terlebih dahulu, terutama perubahan yang dapat memengaruhi struktur URL, implementasi redirect, akses crawler, atau visibilitas halaman pada mesin pencari.

Setelah rekomendasi disetujui, detail tindakan diteruskan kepada tim development untuk diimplementasikan. Status implementasi dan hasil tindak lanjut kemudian diperbarui dalam spreadsheet audit.

---

## Deliverables

Hasil pekerjaan didokumentasikan dalam spreadsheet yang mencakup:

- Laporan indexing dari Google Search Console
- Klasifikasi isu pada tingkat URL
- Analisis Technical SEO
- Catatan pemeriksaan URL
- Rekomendasi tindakan untuk setiap isu
- Rekomendasi redirect
- Rekomendasi crawling dan indexing
- Status implementasi
- Catatan tindak lanjut untuk PM dan tim development

---

## Tools yang Digunakan

| Tools | Penggunaan |
|---|---|
| Google Search Console | Pemeriksaan laporan indexing, URL inspection, dan validasi status halaman |
| Google Sheets | Pengolahan data, klasifikasi isu, dokumentasi audit, serta pelacakan implementasi |
| Google Search | Pemeriksaan tampilan halaman pada hasil pencarian dan validasi indeks |
| Website Analysis | Evaluasi kondisi halaman, internal linking, redirect, meta robots, dan aspek Technical SEO lainnya |

---

## Keahlian yang Ditunjukkan

- Technical SEO
- Google Search Console
- Google Indexing Analysis
- Crawling Analysis
- URL Auditing
- 404 Error Analysis
- Redirect Analysis
- Robots.txt Analysis
- Noindex Analysis
- Internal Linking Analysis
- SEO Documentation
- Google Sheets
- Cross-functional Collaboration
- Technical SEO Recommendations

---

## Catatan Portofolio

Proyek ini dibuat sebagai dokumentasi kemampuan dalam melakukan audit Technical SEO, menganalisis kendala crawling dan indexing, menyusun rekomendasi berbasis data, serta berkoordinasi dengan stakeholder dalam proses implementasi perbaikan.

Seluruh informasi sensitif telah dianonimkan untuk menjaga kerahasiaan klien dan data bisnis.
