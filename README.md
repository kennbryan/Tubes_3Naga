# Platform Pemesanan Ruang Kelas dan Meeting - Telkom University

## Kontributor

### 1. Ferdiansyah Adi Saputra
- **NIM**: 102022330113
- **Username GitHub**: [ferdayyaye](https://github.com/ferdayyaye)
- **Peran**: Fitur Utama yang Dikerjakan: Login dan Registrasi, Dashboard Utama, Edit Profile 

#### Kesesuaian antara Desain dan Implementasi
- **Deskripsi**: Implementasi seluruh fitur dilakukan sesuai dengan desain awal yang tertuang dalam use case dan ERD. Tabel `users`, `bookings`, serta logika `role-based access control` telah dibuat dan dihubungkan dengan baik sesuai diagram kelas.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Semua fitur yang saya kerjakan telah sesuai 100% dengan desain awal, baik dari sisi struktur data maupun alur penggunaan.

#### Kualitas Fitur CRUD (Fungsi dan Validasi)
- **Deskripsi**:
  - **Create**: Registrasi pengguna dan pembuatan riwayat pemesanan otomatis saat pemesanan dilakukan.
  - **Read**: Tampilan data pengguna dan riwayat pemesanan masing-masing.
  - **Update**: Edit profil, pembatalan pemesanan oleh user.
  - **Delete**: Penghapusan akun (admin) atau pemesanan (user).
  - **View** meliputi form login, registrasi, halaman profil, dan riwayat pemesanan.
  - **Validasi**: Server-side validasi aktif untuk semua form penting, termasuk format email, password, dan input waktu pembatalan.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Fitur CRUD berjalan sempurna, seluruh validasi diterapkan, dan tidak ditemukan error dalam pengujian.

#### Implementasi API (Route, Controller, JSON Response)
- **Deskripsi**:
  - **Endpoint**: `/api/users`, `/api/users/{id}`, `/api/bookings/history`
  - Menggunakan controller untuk generate JSON response dengan format.
  - Validasi pada input ID dan autentikasi JWT atau session-based login diterapkan.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Semua endpoint berjalan dengan baik, aman, dan sesuai prinsip RESTful API.

#### Git & Kolaborasi Tim
- **Deskripsi**: Komitmen dilakukan secara rutin dengan deskripsi jelas, terutama di branch `feature/auth` dan `feature/user-management`. Estimasi jumlah commit > 10.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Commit saya menunjukkan progres fitur secara jelas, terstruktur, dan konsisten dalam kolaborasi tim.

---

### 2. Syarief Saleh Madhy
- **NIM**: 102022300201
- **Username GitHub**: [Syarief10](https://github.com/Syarief10)
- **Peran**: Fitur Utama yang Dikerjakan: Manajemen Jadwal Ruangan, Pemilihan & Pemesanan Ruang, Pencarian Ruang.

#### Kesesuaian antara Desain dan Implementasi
- **Deskripsi**: Seluruh fitur telah diimplementasikan sesuai dengan use case dan class diagram yang ditetapkan, terutama penggunaan filter pencarian dan integrasi dengan jadwal.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Implementasi fitur sesuai dengan rancangan desain, termasuk pencegahan bentrokan jadwal.

#### Kualitas Fitur CRUD (Fungsi dan Validasi)
- **Deskripsi**:
  - **Create**: Pemesanan ruang oleh user.
  - **Read**: Menampilkan ruang berdasarkan filter.
  - **Update**: Perubahan waktu pemesanan.
  - **Delete**: Penghapusan pemesanan (jika batal).
  - **Validasi** mencakup ketersediaan ruang dan waktu yang tidak bentrok.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Semua fungsi CRUD berjalan dengan baik, sistem validasi berhasil mencegah konflik jadwal, dan pengujian tidak menemukan bug.

#### Implementasi API (Route, Controller, JSON Response)
- **Deskripsi**:
  - **Endpoint**: `/api/rooms`, `/api/rooms/{id}`, `/api/bookings/available`
  - JSON response dinamis berdasarkan filter pencarian ruang.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Endpoint dapat diakses, responsif, dan telah divalidasi input filter (kapasitas, waktu, fasilitas).

#### Git & Kolaborasi Tim
- **Deskripsi**: Aktif di branch `feature/booking-management`, total >10 commit dengan deskripsi progres yang jelas.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Kontribusi saya konsisten dan seluruh hasil pekerjaan tercermin dalam riwayat commit.

---

### 3. Kenneth Bryan
- **NIM**: 102022330093
- **Username GitHub**: [kennbryan](https://github.com/kennbryan)
- **Peran**: Fitur Utama yang Dikerjakan: Verifikasi & Persetujuan Pemesanan, Pembatalan Ruangan, Manajemen Data Ruang.

#### Kesesuaian antara Desain dan Implementasi
- **Deskripsi**: Implementasi fitur admin sesuai dengan rancangan awal, termasuk pembagian hak akses untuk memverifikasi dan menolak pemesanan. Struktur tabel ruang dan notifikasi sesuai dengan ERD.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Semua fitur berjalan sesuai desain dengan logika otorisasi admin yang tepat.

#### Kualitas Fitur CRUD (Fungsi dan Validasi)
- **Deskripsi**:
  - **Create**: Tambah data ruang dan notifikasi.
  - **Read**: Daftar ruang dan notifikasi status pemesanan.
  - **Update**: Persetujuan pemesanan.
  - **Delete**: Hapus ruang jika tidak digunakan lagi.
  - Validasi dilakukan pada pengisian kapasitas, deskripsi, dan ID relasi.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Semua fitur CRUD berjalan baik dan validasi berhasil mencegah kesalahan input.

#### Implementasi API (Route, Controller, JSON Response)
- **Deskripsi**: Endpoint untuk Pembatalan dan Histori Pesanan (`GET /api/pembatalan`, `GET /api/book`, `GET /api/jadwal`, dll.), dengan otorisasi pada level controller.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: API telah tersedia, dapat diakses, dan menerapkan praktik REST yang aman.

#### Git & Kolaborasi Tim
- **Deskripsi**: Total kontribusi saya terdiri dari 11 commit yang mencerminkan alur kerja yang sistematis.
- **Penilaian Diri**: A (86–100)
- **Justifikasi**: Seluruh riwayat dan detail pengerjaan dapat diverifikasi secara transparan melalui repositori GitHub.

---

## Penjelasan Proyek
Tugas ini bertujuan merancang dan mengembangkan platform pemesanan ruang kelas dan ruang meeting berbasis website di Telkom University sebagai solusi atas sistem manual yang tidak efisien. Proses pemesanan yang dilakukan melalui email atau tatap muka sering menimbulkan bentrokan jadwal dan pemanfaatan ruang yang tidak optimal. Platform yang dikembangkan akan menyediakan fitur pencarian dan filter ruang, tampilan jadwal ketersediaan, dan notifikasi status pemesanan. Sistem juga akan menerapkan validasi jadwal otomatis untuk mencegah bentrokan. Platform ini akan melayani dua jenis pengguna: pengguna umum (mahasiswa, dosen, staf) yang dapat memesan dan memantau status, serta administrator yang memverifikasi permintaan dan mengelola jadwal melalui dasbor terpadu.
