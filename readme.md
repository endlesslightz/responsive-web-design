

# Responsive Web Design dengan CSS Native, Flexbox, dan Grid

Proyek ini adalah contoh sederhana yang menjelaskan konsep **Responsive Web Design** menggunakan CSS native, Flexbox, dan CSS Grid. Tujuannya adalah untuk membantu pemula dan pengembang web memahami cara membangun tata letak web yang dapat menyesuaikan diri dengan berbagai ukuran layar, mulai dari perangkat seluler hingga desktop.

## Daftar Isi
- [Tentang Responsive Web Design](#tentang-responsive-web-design)
- [Teknik dan Tools](#teknik-dan-tools)
  - [CSS Media Queries](#css-media-queries)
  - [Flexbox](#flexbox)
  - [Grid](#grid)
- [Contoh Struktur](#contoh-struktur)
- [Lisensi](#lisensi)


## Tentang Responsive Web Design

**Responsive Web Design (RWD)** adalah pendekatan untuk membuat desain web yang dapat menyesuaikan tampilannya dengan ukuran dan orientasi layar perangkat pengguna. RWD menggabungkan penggunaan:
- *Fluid grid layouts* yang proporsional,
- Media queries untuk mendeteksi lebar layar, dan
- Gambar serta konten yang dapat menyesuaikan ukuran.

RWD memungkinkan website terlihat optimal dan fungsional di berbagai perangkat tanpa memerlukan pembuatan beberapa versi situs.

## Teknik dan Tools

### CSS Media Queries
Media queries memungkinkan kita untuk menerapkan aturan CSS berdasarkan kondisi tertentu, seperti lebar layar. Ini adalah komponen kunci dalam RWD untuk membuat elemen beradaptasi dengan ukuran layar yang berbeda.

```css
/* CSS Media Query sederhana */
@media (max-width: 768px) {
  .container {
    width: 100%;
    padding: 10px;
  }
}
```

### Flexbox
Flexbox adalah metode layout berbasis kolom atau baris yang cocok untuk membuat tata letak dinamis. Dengan Flexbox, kita bisa membuat elemen-elemen saling menyesuaikan, mendukung align dan distribution yang fleksibel di berbagai perangkat.

```css
.container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

.item {
  flex: 1 1 200px; /* Menentukan elemen berukuran minimal 200px */
}
```

### Grid
CSS Grid adalah sistem tata letak dua dimensi yang memungkinkan kita mengatur elemen dalam baris dan kolom. Grid sangat kuat untuk membangun tata letak yang lebih kompleks dan responsif.

```css
.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 20px;
}

.item {
  background-color: #f2f2f2;
  padding: 20px;
}
```

## Contoh Struktur

```
responsive-web-design
├── index.html
├── style.css
└── README.md
```

- **index.html**: Berisi struktur HTML dasar untuk tata letak halaman.
- **style.css**: Berisi kode CSS untuk mengatur responsivitas menggunakan Media Queries, Flexbox, dan Grid.

## Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE).

