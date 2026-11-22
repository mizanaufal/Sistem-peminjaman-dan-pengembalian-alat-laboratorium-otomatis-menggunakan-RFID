# Smart Locker Peminjaman dan Pengembalian Alat Laboratorium Berbasis IoT

## Latar Belakang
Pengelolaan peminjaman dan pengembalian alat laboratorium secara manual berpotensi menimbulkan berbagai permasalahan, seperti kesulitan dalam memantau ketersediaan alat, pencatatan transaksi yang kurang terorganisasi, serta keterlambatan dalam mengetahui status peminjaman. Selain itu, proses peminjaman yang masih bergantung pada pengawasan petugas dapat mengurangi efisiensi penggunaan fasilitas laboratorium.

Oleh karena itu, dikembangkan **Smart Locker berbasis Internet of Things (IoT)** yang memanfaatkan ESP32 sebagai mikrokontroler utama. Sistem ini mengintegrasikan RFID sebagai identifikasi pengguna, sensor ultrasonik untuk mendeteksi keberadaan alat, servo motor sebagai mekanisme pengunci, serta MQTT untuk komunikasi dan pemantauan status perangkat secara real-time.

## Tujuan
1. Mengembangkan sistem peminjaman dan pengembalian alat laboratorium secara otomatis menggunakan teknologi RFID.
2. Mempermudah proses identifikasi pengguna melalui kartu RFID yang telah terdaftar.
3. Memantau ketersediaan dan jumlah stok alat menggunakan sensor dan sistem pencatatan otomatis.
4. Mencatat waktu peminjaman dan pengembalian alat menggunakan modul RTC.
5. Mengintegrasikan protokol MQTT untuk mengirimkan informasi status stok dan riwayat transaksi.
6. Meningkatkan efisiensi dan keteraturan pengelolaan inventaris alat laboratorium.

## Manfaat
1. **Efisiensi Peminjaman:** Mempermudah pengguna dalam melakukan peminjaman dan pengembalian alat tanpa proses pencatatan manual.
2. **Pemantauan Stok:** Memudahkan pemantauan jumlah alat yang tersedia dan sedang dipinjam.
3. **Keamanan Akses:** Membatasi akses loker hanya kepada pengguna yang memiliki kartu RFID terdaftar.
4. **Pencatatan Otomatis:** Menyimpan informasi waktu dan aktivitas peminjaman maupun pengembalian alat.
5. **Pemantauan Jarak Jauh:** Memungkinkan pemantauan status perangkat melalui komunikasi MQTT.
6. **Pengelolaan Inventaris:** Membantu laboratorium dalam mengelola dan mengawasi penggunaan inventaris secara lebih terstruktur.

## Teknologi yang Digunakan
- ESP32
- RFID RC522
- Ultrasonic Sensor HC-SR04
- Servo Motor
- LCD I2C 16x2
- RTC DS1307
- LED Indicator
- Buzzer
- Wi-Fi
- MQTT Protocol (HiveMQ Broker)
- Arduino Framework / PlatformIO

## Fitur Utama
- Autentikasi pengguna menggunakan kartu RFID.
- Peminjaman dan pengembalian alat otomatis.
- Deteksi keberadaan alat di dalam loker.
- Penghitungan stok alat secara otomatis.
- Pencatatan waktu peminjaman dan durasi penggunaan.
- Indikator status menggunakan LED dan buzzer.
- Monitoring stok melalui MQTT.
- Pencatatan log transaksi melalui MQTT.
- Remote unlock melalui perintah MQTT.

## Pengembangan
Proyek ini dikembangkan menggunakan ESP32 dan dapat disimulasikan melalui Wokwi untuk menguji fungsi serta integrasi antarperangkat sebelum diterapkan pada perangkat keras sebenarnya.
