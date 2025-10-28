# Proyek Latihan Layout HTML & CSS Responsif

Ini adalah proyek latihan sederhana yang mendemonstrasikan pembuatan layout web responsif menggunakan HTML semantik dan CSS Flexbox. Proyek ini menerapkan pendekatan **Mobile-First**, di mana layout default dirancang untuk perangkat seluler dan kemudian disesuaikan untuk layar yang lebih besar (desktop) menggunakan media query.

## Fitur Utama

- **Struktur HTML Semantik:** Menggunakan tag HTML5 modern seperti `<header>`, `<footer>`, `<section>`, `<aside>`, dan `<main>` untuk struktur halaman yang jelas dan mudah dibaca.
- **Desain Responsif (Mobile-First):** Tampilan dioptimalkan untuk perangkat seluler terlebih dahulu, kemudian beradaptasi ke layar yang lebih besar pada breakpoint `1024px`.
- **Layout CSS Flexbox:** `display: flex` digunakan secara ekstensif untuk mengatur tata letak utama, termasuk navigasi dan bagian konten, serta untuk perataan item.
- **Box Model Konsisten:** Menerapkan `box-sizing: border-box;` secara global (`*`) untuk memastikan bahwa properti `padding` dan `border` disertakan dalam perhitungan total `width` dan `height`, mencegah masalah _overflow_ yang umum terjadi.

## Perilaku Layout

Proyek ini memiliki dua status layout utama:

### 1. Tampilan Seluler (Default / Lebar < 1024px)

- **Header & Navigasi:** Konten di dalam header (judul "Header" dan navigasi) ditumpuk secara vertikal (`flex-direction: column`).
- **Menu Navigasi:** Tombol "Menu" disusun secara vertikal dan memenuhi lebar layar.
- **Konten Utama:** Bagian `<aside>` (sidebar) dan `<main>` (konten) ditumpuk secara vertikal (`flex-direction: column`), masing-masing dengan lebar `100%`.

### 2. Tampilan Desktop (Lebar >= 1024px)

- **Menu Navigasi:** Tombol "Menu" secara otomatis berubah menjadi susunan horizontal (`flex-direction: row`), terpusat, dan memiliki sudut membulat (`border-radius: 10px`).
- **Konten Utama:** Layout berubah menjadi horizontal. Bagian `<aside>` mengambil `25%` lebar dan bagian `<main>` mengambil `75%` lebar, sehingga keduanya tampil berdampingan.

## Teknologi yang Digunakan

- **HTML5**
- **CSS3**
  - Flexbox
  - Media Queries
  - Box Model

## Cara Menggunakan

1.  Simpan kode HTML di atas sebagai `index.html`.
2.  Simpan kode CSS di atas sebagai `style.css` di folder yang sama dengan `index.html`.
3.  Buka file `index.html` di browser web pilihan Anda.
4.  Ubah ukuran jendela browser (atau gunakan Developer Tools) untuk melihat perubahan layout dari seluler ke desktop pada breakpoint `1024px`.
