# HerYaml — Sing-box anti-iklan

Profil Sing-box di repositori ini memblokir domain iklan, pelacak, phishing, malware, judi, dan scam sebelum aplikasi dapat tersambung. Perlindungan berlaku untuk aplikasi Android melalui mode VPN/TUN.

## Pilih file

- `singbox_android.json` — profil utama dengan akun proxy dan proteksi anti-iklan.
- `singbox_direct_adblock.json` — profil tanpa proxy; hanya DNS aman dan blokir iklan/pelacak. Gunakan bila tidak membutuhkan proxy.

## Cara pasang di aplikasi Sing-box Android

1. Unduh salah satu file JSON dari repositori ini.
2. Buka aplikasi **sing-box**.
3. Buka **Profiles**.
4. Tekan tombol **+** lalu pilih **Import from file**.
5. Pilih file JSON yang sudah diunduh.
6. Aktifkan profil hasil impor.
7. Tekan **Start** dan setujui izin VPN Android.

Sing-box akan membuat VPN lokal. Semua trafik aplikasi melewati aturan profil. Domain iklan dan domain berbahaya akan ditolak.

## Jika aplikasi internet bermasalah

1. Pastikan profil aktif dan layanan Sing-box sudah **Start**.
2. Coba ganti ke `singbox_direct_adblock.json` untuk memastikan masalah bukan dari akun proxy.
3. Jangan mematikan aturan secara massal. Laporkan nama aplikasi dan domain/error bila tersedia agar pengecualian dibuat spesifik.

## Catatan keamanan

- Jangan unggah file profil ke layanan publik. `singbox_android.json` dapat berisi akun proxy.
- Perbarui profil dari repositori ini secara berkala.
- Domain pembayaran, perbankan, QRIS, ShopeePay, streaming, dan layanan resmi diprioritaskan agar tidak terkena blokir iklan.
- Aturan anti-malware memakai indikator spesifik dan diverifikasi untuk menekan false positive.
