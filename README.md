## React Native Multi-Mini-Apps Demo 📱
Aplikasi React Native interaktif yang menggabungkan empat komponen mini dalam satu antarmuka berbasis navigasi Bottom Tab Bar kustom. Proyek ini dirancang untuk mendemonstrasikan manajemen state lokal, pengiriman props, arsitektur berbasis komponen, serta navigasi sederhana tanpa pustaka eksternal.

## ✨ Fitur & Modul Komponen
Aplikasi ini terbagi menjadi 4 tab utama yang masing-masing memuat fungsionalitas berbeda:

🔢 Counter (CounterApp):
Aplikasi penghitung angka interaktif untuk melatih manipulasi state numerik dasar (tambah, kurang, dan reset).
❤️ Like Button (LikeButton):
Demonstrasi komponen reusable (dapat digunakan kembali) dengan pengiriman props (initialCount).
Menampilkan tiga instance tombol like dengan jumlah awal berbeda (42, 128, dan 7) yang mengelola state-nya masing-masing secara independen.
🌙 Theme (DarkModeApp):
Demonstrasi pergantian tema tampilan secara dinamis (Light Mode dan Dark Mode) menggunakan boolean state.
✅ Todo (TodoApp):
Aplikasi pencatat daftar tugas sederhana untuk mempraktikkan manipulasi state bertipe array (menambah, menandai selesai, dan menghapus tugas).

## 📂 Struktur Proyek
Pastikan struktur direktori proyek Anda tersusun seperti berikut agar impor komponen berjalan lancar:
├── App.js                      # Komponen utama & pengatur navigasi tab
└── components/
    ├── CounterApp.js           # Komponen penghitung
    ├── LikeButton.js           # Komponen tombol like dengan props
    ├── DarkModeApp.js          # Komponen pengatur tema gelap/terang
    └── TodoApp.js              # Komponen daftar tugas (To-Do List)


## 🛠️ Konsep React Native yang Diterapkan
- Custom Tab Navigation: Menggunakan useState untuk melacak tab yang aktif (activeTab) dan pernyataan switch-case (renderContent) untuk merender komponen secara kondisional.
- Component Reusability & Props: Menggunakan ulang komponen <LikeButton /> beberapa kali dalam satu layar dengan nilai props yang berbeda.
- Core Components: Memanfaatkan SafeAreaView, View, Text, TouchableOpacity, dan StyleSheet untuk membangun tata letak yang responsif dan rapi.
- Dynamic Styling: Mengubah gaya tab aktif secara dinamis menggunakan kombinasi array style ([styles.tab, activeTab === tab.key && styles.tabActive]).
