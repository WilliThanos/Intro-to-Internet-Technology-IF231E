# UMNLife 
UMNLife - Kelompok 1 | UTS PTI (IF231 - E, EL)
- Hansen (00000060325)
- Liusianto (00000061560)
- Marselino Lengyu Pantouw (00000061909)
- Prudence Tendy (00000060765)
- William Rayhan Harsono (00000061964)

## JAM
Jam akan otomatis berjalan mengambil current time dari player dan berjalan sesuai dengan aturan game dimana 1 detik = 1 menit.

## BACKGROUND
Background akan berubah sesuai dengan waktu
  - Jam 19 - 4.59 (< 5): selamat malam
  - Jam 5 - 10.59 (< 11): selamat pagi
  - Jam 11 - 14.59 (< 15): selamat siang
  - Jam 15 - 18.59 (< 19): Selamat sore
  - Jam 19 - 4.59: selamat malam
  
## GAMBAR KARAKTER
  - Gender yang dipilih sebelum bermain
  - Melakukan aktivitas tertentu sesuai gender

## BUTTON
  - Pojok kanan bawah: dapat digunakan untuk memutar musik (musik default, hanya 1). Ketika musik sedang berjalan, tekan tombol musik sekali lagi untuk pause/mematikan musik
  - Pojok kanan atas dalam game: minimize, maximize, close
    - minimize: keluar dari fullscreen
    - maximize: memasukki mode fullscreen. Klik minimize (-) untuk keluar dari mode fullscreen
    - close: kembali ke index.html

## CARA BERMAIN
- Membuka website / file index.html dan akan berada di tampilan home
- Sebelum bermain, masukkan nama dan pilih karakter
- Tekan tombol Play! untuk bermain dan diarahkan ke tampilan game
- Terdapat 6 progress bar. Setiap progress bar memiliki namanya masing-masing dan dapat dilihat dengan mengarahkan mouse ke bar tersebut
- Objektif dari permainan UMN Life adalah menyelesaikan studi hingga akhir semester 8. 
- Pastikan juga setiap progress bar tidak mencapai kosong/0.

## PERATURAN GAME
Terdapat 6 progress bar yang dapat di-isi oleh player dengan melakukan kegiatan yang sesuai melalui button di bawah.
 Progress bar
  - Bertambah: progress bar akan bertambah ketika karakter melakukan aktivitas
  - Menambah: melakukan aktivitas tertentu akan menambah progress lain
  - Mengurangi: mengurangi progress lain
  - Berkurang: mengurangi progress sendiri
  - Fitur tambahan: fitur unik yang menjadi tambahan pada progress tertentu
  - Game over: kondisi dimana game berakhir karena suatu kondisi
 
### 1) MAKAN
  - Bertambah: ketika karakter makan
    - nasi += 5 
    - snack += 2.5 
    - buah += 3.7
  - Menambah: ketik karakter makan, progress kesehatan juga akan bertambah
  - Mengurangi: ketika karakter makan, progress tidur, main, belajar, minum akan berkurang.
  - Berkurang: ketika karakter tidak diberi makan selama 15 detik (lapar, butuh makan)
  - Game over: ketika progress makan mencapai angka 0, game akan berakhir karena karakter mati akibat **LAPAR**
    dan memulai ulang permainan (semua progress hilang).
   
### 2) TIDUR
  - Bertambah: ketika karakter tidur (tidur += 5)
  - Menambah: ketik karakter tidur, progress kesehatan juga akan bertambah
  - Mengurangi: ketika karakter tidur, progress makan, main, belajar, haus akan berkurang
  - Berkurang: ketika karakter tidak tidur selama 20 detik (capek, butuh tidur)
  - Fitur tambahan: ketika progress tidur karakter mencapai angka 0, karakter akan otomatis
    memasuki mode **TIDUR** yang lebih lama
     
### 3) MAIN
  - Bertambah: ketika karakter main (main += 5)
  - Mengurangi: ketika karakter main, progress makan, tidur, belajar, minum, dan kesehaatan akan berkurang
  - Berkurang: ketika karakter tidak main selama 12 detik (bosan, butuh main)

### 4) BELAJAR
  - Bertambah: ketika karakter belajar (belajar += 2.5)
  - Mengurangi: ketika karakter belajar, progress makan, tidur, main, minum, kesehatan akan berkurang
  - Berkurang: ketika karakter tidak belajar selama 60 detik (kurang ilmu, butuh belajar)
  - Fitur tambahan: 
   - Setiap karakter berhasil menyelesaikan semester, progress untuk memenuhi semester selanjutnya
     akan bertambah 1. Sehingga karakter butuh belajar lebih banyak lagi supaya dapat meningkatkan progress belajar
   - Ketika karakter berhasil menyelesaikan hingga akhir semester 8, karakter dianggap **LULUS**
     lulus dari Universitas Multimedia Nusantara dan akan dikembalikan ke halaman awal

### 5) KESEHATAN
  - Bertambah: ketika karakter 
    - sehat/mengunjungi dokter (sehat += 4)
    - karakter makan (sehat += 1)
    - karakter tidur (sehat += 2)
    - karakter minum (sehat += 0.5)
  - Mengurangi: ketika karakter mengunjungi dokter, progress makan, tidur, main, belajar, minum akan berkurang
  - Berkurang: ketika karakter tidak mengunjungi dokter/berobat, tidak makan, tidak tidur (sakit, butuh berobat/ke dokter)
  - Game over: ketika progress kesehatan mencapai angka 0, game akan berakhir karena 
    karakter **MATI** akibat sakit dan memulai ulang permainan. (semua progress hilang)
    
### 6) MINUM
  - Bertambah: ketika karakter minum (minum += 4)
  - Menambah: ketik karakter minum, status kesehatan juga akan bertambah
  - Mengurangi: 
    - ketika karakter minum, progress main akan berkurang. 
    - ketika karakter tidak minum dalam 11 detik, progress sehat dan belajar akan dikurangi 
      (dehidrasi membuat kurangnya cairan bagi tubuh dan mengurangi fokus belajar)
  - Berkurang: ketika karakter tidak minum selama 11 detik (haus, butuh minum)
