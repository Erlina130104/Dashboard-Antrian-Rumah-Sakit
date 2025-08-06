Sistem Antrian Rumah Sakit Otomatis Berbasis Arduino Mega
Proyek ini merupakan sistem antrian elektronik yang menggunakan Arduino Mega, DFPlayer Mini, dan LCD 16x4 untuk memutar suara nomor antrian secara otomatis ketika tombol ditekan. Sistem ini cocok untuk digunakan di ruang tunggu, klinik, atau tempat layanan publik skala kecil.

 Fitur Utama
- Menampilkan nomor antrian pengguna di LCD
- Menyebutkan nomor antrian melalui DFPlayer Mini
- Menampilkan nomor yang sedang dipanggil
- Tombol untuk ambil antrian, lihat status, dan navigasi suara
Komponen yang Digunakan
1.	Arduino Mega 
Arduino mega yang digunakan berjumlah 1 dan berfungsi untuk kontrol utama.

2.	LCD 16X4 I2C 
Berfungsi untuk menampilkan teks.

3.	DFPlayer Mini
Berfungsi untuk memutar file MP3 suara

4.	Speaker
Berfungsi sebagai output suara

5.	Push Button      
Berfungsi sebagai Navigasi & kontrol 

6.	MicroSD Card     
Berfungsi untuk menyimpan file audio (misal: 001.mp3 - 010.mp3) 

7.	Papan USB        
Untuk power atau koneksi komputer 

 Konfigurasi Pin (Default)
-	DFPlayer RX , pin Arduino 10         
-	DFPlayer TX, pin Arduino 11          
-	Button Next, pin arduino  2  
-	Button Previous, pin arduino 4         
-	Button Ambil Antrian, pin arduino  5    
-	Button Status Layar, pin arduino  3     

  File dalam Proyek
- arduino.ino → Sketch utama Arduino 
- README.md → Dokumentasi ini

 Cara Kerja Singkat
1. Saat tombol Ambil Antrian ditekan:
   - Nomor antrian bertambah
   - Nomor ditampilkan di LCD
   - Suara diputar oleh DFPlayer Mini (misal: “Nomor: 1”)
2. Tombol status menampilkan antrian yang sedang dipanggil
3. Tombol next/previous bisa memainkan ulang suara nomor

 Cara Menyimpan File MP3
 File disimpan dalam MicroSD card dalam format:
001.mp3 → "Nomor 1"
002.mp3 → "Nomor 2"
...
010.mp3 → "Nomor 10"

Catatan Tambahan
- Proyek ini cocok digabungkan dengan sistem dashboard cloud untuk antrian online
- Bisa ditambahkan dengan ESP32 untuk notifikasi ke cloud secara real-time


