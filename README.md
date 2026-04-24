# Jalanin Aja — Website Rental Mobil

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white"/>
  <img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
</p>

> Tugas Pemrograman Web — Website rental mobil statis berbasis HTML, CSS, dan JavaScript dengan nama brand **Jalanin Aja**, menyediakan tampilan layanan sewa kendaraan yang modern dan responsif.

---

##  Daftar Isi

- [Tentang Proyek](#-tentang-proyek)
- [Teknologi yang Digunakan](#-teknologi-yang-digunakan)
- [Struktur File](#-struktur-file)
- [Halaman & Fitur](#-halaman--fitur)
- [Library Eksternal](#-library-eksternal)
- [JavaScript (main.js)](#️-javascript-mainjs)
- [Cara Menjalankan](#-cara-menjalankan)

---

##  Tentang Proyek

**Jalanin Aja** adalah website profil perusahaan rental mobil fiktif yang dibuat sebagai tugas mata kuliah Pemrograman Web. Website ini sepenuhnya bersifat **front-end only** (statis) — belum terhubung dengan back-end atau database, sehingga form pemesanan dan kontak belum berfungsi secara fungsional.

Website ini menampilkan:
- Profil perusahaan dan layanan rental mobil
- Galeri armada kendaraan lengkap dengan harga
- Sistem reservasi dalam bentuk form statis
- Halaman blog, tim, dan testimoni pelanggan

---

##  Teknologi yang Digunakan

| Teknologi | Versi | Fungsi |
|---|---|---|
| **HTML5** | — | Struktur halaman |
| **CSS3 / SCSS** | — | Styling dan layout kustom |
| **Bootstrap** | 5.0.0 | Framework CSS responsif & komponen UI |
| **jQuery** | 3.6.4 | Manipulasi DOM dan event handling |
| **WOW.js + Animate.css** | — | Animasi elemen saat di-scroll |
| **Owl Carousel** | — | Slider gambar dan kartu mobil |
| **CounterUp + Waypoints** | — | Animasi angka statistik |
| **jQuery Easing** | — | Efek smooth scroll |
| **Font Awesome** | 5.15.4 | Ikon-ikon di seluruh halaman |
| **Bootstrap Icons** | 1.4.1 | Ikon tambahan |
| **Google Fonts** | — | Font `Lato` dan `Montserrat` |

---

##  Struktur File

```
tugas-pweb-rental-mobil/
│
├── index.html            # Halaman Beranda (halaman utama)
├── about.html            # Halaman Tentang Kami
├── service.html          # Halaman Layanan
├── cars.html             # Halaman Armada Mobil
├── blog.html             # Halaman Blog & Tips
├── contact.html          # Halaman Kontak
├── feature.html          # Halaman Fitur Kami
├── team.html             # Halaman Tim Kami
├── testimonial.html      # Halaman Testimoni Pelanggan
│
├── css/
│   ├── bootstrap.min.css # Bootstrap yang telah dikustomisasi
│   └── style.css         # CSS kustom utama
│
├── js/
│   └── main.js           # JavaScript kustom (animasi, carousel, dll)
│
├── lib/                  # Library pihak ketiga
│   ├── animate/          # Animate.css
│   ├── owlcarousel/      # Owl Carousel JS & CSS
│   ├── wow/              # WOW.js
│   ├── counterup/        # CounterUp.js
│   ├── easing/           # jQuery Easing
│   └── waypoints/        # Waypoints.js
│
├── img/                  # Semua aset gambar
└── scss/                 # Source file SCSS
    └── bootstrap.scss
```

---

##  Halaman & Fitur

### `index.html` — Beranda
Halaman utama dan terlengkap. Berisi:
- **Topbar** — Info kontak dan ikon sosial media (hanya tampil di layar XL)
- **Navbar Sticky** — Logo teks, menu navigasi, dropdown "Lainnya", tombol "Mulai Sewa"
- **Hero Carousel** — 2 slide gambar dengan form reservasi (pilih mobil, lokasi, tanggal, jam)
- **Section Keunggulan** — 4 fitur unggulan dengan layout simetris (kiri-tengah-kanan)
- **Section Tentang** — Visi & misi, statistik 10 tahun pengalaman, profil pendiri
- **Fact Counter** — Animasi angka: 420+ pelanggan, 67+ unit, 70+ mitra, 911+ km
- **Section Layanan** — 6 kartu layanan dalam grid 3 kolom
- **Section Proses** — 3 langkah: Hubungi → Pilih Mobil → Nikmati Perjalanan
- **Footer** — Subscribe email, tautan cepat, jam kerja, info kontak

### `about.html` — Tentang Kami
Halaman khusus profil perusahaan dengan section visi, misi, dan galeri foto.

### `service.html` — Layanan
Menampilkan 6 layanan utama: Pemesanan Mudah, Harga Kompetitif, Sewa Lepas Kunci, Asuransi Perjalanan, Antar Kota, dan Gratis Antar Unit.

### `cars.html` — Armada Mobil
- Filter kategori kendaraan (Semua / SUV / Sedan / Electric)
- **Owl Carousel** responsif menampilkan kartu tiap mobil
- Informasi per unit: nama, harga/hari, jumlah kursi, kapasitas bagasi, transmisi, jenis BBM
- Contoh armada: Mercedes Benz R3 (Rp 1.500.000/hari), Tesla Model S Plaid (Rp 2.500.000/hari)

### `blog.html` — Blog & Tips
Kartu artikel perjalanan dengan gambar, tanggal, jumlah komentar, dan tombol baca selengkapnya.

### `contact.html` — Kontak
- 4 kartu info: Alamat, Email, Telepon, WhatsApp
- Form kontak (nama, email, subjek, pesan)
- Embed Google Maps via `<iframe>`

### `feature.html` — Fitur Kami
Menampilkan keunggulan layanan secara detail, dilengkapi section **FAQ accordion** (Bootstrap Collapse).

### `team.html` — Tim Kami
Grid kartu anggota tim dengan foto, nama, jabatan, dan ikon sosial media.

### `testimonial.html` — Testimoni
Owl Carousel testimoni pelanggan dengan bintang rating dan ulasan teks.

---

##  Library Eksternal

Semua library dimuat melalui CDN atau folder `lib/`:

```html
<!-- CDN -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.4/jquery.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0/dist/js/bootstrap.bundle.min.js"></script>

<!-- Local lib/ -->
<script src="lib/wow/wow.min.js"></script>
<script src="lib/easing/easing.min.js"></script>
<script src="lib/waypoints/waypoints.min.js"></script>
<script src="lib/counterup/counterup.min.js"></script>
<script src="lib/owlcarousel/owl.carousel.min.js"></script>
```

---

##  JavaScript (`main.js`)

Semua kode dikemas dalam IIFE jQuery agar tidak mencemari scope global:

```javascript
(function ($) {
    "use strict";

    // 1. Hilangkan spinner loading setelah halaman siap
    setTimeout(() => $('#spinner').removeClass('show'), 1);

    // 2. Aktifkan animasi scroll WOW.js
    new WOW().init();

    // 3. Navbar sticky + shadow saat scroll lebih dari 200px
    $(window).scroll(function () {
        if ($(this).scrollTop() > 200) {
            $('.sticky-top').addClass('shadow-sm').css('top', '0px');
        } else {
            $('.sticky-top').removeClass('shadow-sm').css('top', '-100px');
        }
    });

    // 4. Carousel armada mobil (responsif: 1–3 item)
    $(".categories-carousel").owlCarousel({ loop: true, margin: 25, ... });

    // 5. Carousel testimoni (responsif: 1–2 item, dengan dots)
    $(".testimonial-carousel").owlCarousel({ dots: true, autoplay: true, ... });

    // 6. Animasi counter angka statistik (durasi 2 detik)
    $('[data-toggle="counter-up"]').counterUp({ delay: 5, time: 2000 });

    // 7. Tombol Back-to-Top: muncul saat scroll > 300px
    //    Klik → smooth scroll ke atas (efek easeInOutExpo)
    $('.back-to-top').click(function () {
        $('html, body').animate({ scrollTop: 0 }, 1500, 'easeInOutExpo');
    });

})(jQuery);
```

---

##  Cara Menjalankan
arahkan ke folder xampp/htdocs

Buka Xampp Start Apache Saja, Lalu Buka Browser Ketik Berikut

http://localhost/tugas-pweb-rental-mobil
