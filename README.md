# Tugas Akhir Pemodelan Oseanografi Team-19
Repository ini dibuat untuk memenuhi persyaratan Tugas Akhir Praktikum Pemodelan Oseanografi 2022. Repository ini memuat file berupa panduan dan lampiran script python (py) yang nantinya dapat digunakan untuk menjalankan beberapa model pemodelan oseanografi seperti Adveksi-Difusi 2D, Hidrodinamika 1D dan Hidrodinamika 2D. Mandatory library yang digunakan pada praktikum kali ini adalah Numpy, Matplotlib, Siphon, Sys, dan Pprint. Seluruh Script yang dibuat merupakan hasil dari Team 19 Program Studi Oseanografi Universitas Diponegoro 2020. Semoga repository ini dapat bermanfaat!! 
# AUTHORS (Team 19)
- Fadhil Nur Rizqi 26050120140116 B
- Juan Javier 26050120140095 B
- Irene Indah Yuni Simanungkalit 26050120140115 B
- Athanasius Dhento Wilasma 26050120130071 A
- Deno Ferdian 26050120130086 A	
- Shumanty Nathio Simanjuntak 26050120130080 A
- Kalika Padmarani 26050120140043 B
# Cara Penggunaan Script Python
1. Pengguna dapat membuka folder yang berisi kumpulan script python yang dapat dijalankan pada Jupyter Notebook, Visual Studio Code dan Google Colaboratory dalam repository ini. 
2. Setelah dibuka, tampilan script akan muncul seperti di bawah ini.


3. Script python dapat di-copy dan nantinya di-running atau dijalankan pada Jupyter Notebook, Visual Studio Code dan Google Colaboratory.
# MATERI
# Modul Adveksi-Difusi 2 Dimensi
- Pengertian dan Persamaan Pembangun
* Adveksi secara 2 Dimensi merupakan sebuah proses atau mekanisme pergerakan penyebaran atau perluasan materi/property/kuantitas/sifat fisik yang disebabkan oleh aliran fluida akibat dipengaruhi gaya-gaya tertentu dalam arah horizontal.

![adveksi](https://user-images.githubusercontent.com/105922449/169641685-f0855bc6-9db5-4832-8705-ecd86aa21344.JPG)

* Difusi secara 2 Dimensi merupakan sebuah proses transport pasif.

![difusi](https://user-images.githubusercontent.com/105922449/169641827-92a4786a-e6a3-4b84-a8b1-0e163e0ee8e9.JPG)

- Persamaan Adveksi-Difusi terutama 2 Dimensi adalah persamaan matematis yang didesain untuk mempelajari fenomena transpor polutan. Persamaan ini menggambarkan model pemodelan oseanografi yang menggambarkan proses transportasi suatu zat yang dipengaruhi gaya dalam dua dimensi.
# Langkah pengerjaan Script Adveksi-Difusi 2D
1. Pilih satu aplikasi untuk menjalankan script ini seperti Jupyter Notebook, Visual Studio Code atau Google Colaboratory. Kemudian meng-import mandatory library berupa matplotlib.pyplot, numpy dan sys. Dilengkapi juga dengan pendefinisian model yang akan dijalankan.
  
    
2. Selanjutnya dimasukkan parameter awal dan parameter lanjutan untuk perhitungan polutan yang akan digunakan.


3. Setelah itu dilakukan perhitungan dibuat dengan rumusan U dan V untuk mengetahui sebaran dari polutan.


4. Dilanjutkan dengan pembuatan grid agar dalam pembuatan model sebagai boundary atau batas alat bantu untuk menyusun dan mengatur hasil akhir sebaran polutan.


5. Dilakukan iterasi otomatis sampai memenuhi syarat batas kestabilan.


6. Langkah terakhir yaitu membuat script untuk labelling pada grafik output sebaran polutan.


7. Script siap dijalankan

# Modul Hidrodinamika 1 Dimensi
- Pengertian dan Persamaan Pembangun
Pada persamaan hidrodinamika 1 dimensi sederhana persamaan pembangun yang digunakan adalah persamaan kontunuitas dan persamaan momentum atau gerak. Persamaan kontinuitas atau kekelalan massa dimana setiap benda yang masuk dama dengan yang keluar
Momentum merupakan hasil perkalian antara massa dan kecepatan suatu objek. Persamaan momentum didasarkan pada persamaan Hk. II Newton yang berbunyi “setiap benda bermassa yang dikenai gaya akan menimulkan percepatan”. Persamaan Momentum 1 Dimensi Sederhana dapat ditulis:
<img width="125" alt="Screen Shot 2022-05-21 at 17 20 14" src="https://user-images.githubusercontent.com/105969814/169647226-f9265f93-733e-45fd-b973-5e4b68b608ae.png">

* Hidrodinamika merupakan salah satu cabang ilmu pengetahuan yang mempelajari gerak liquid atau gerak fluida cair khususnya gerak air, kondisi hidrodinamika merupakan salah satu aspek yang sangat berpengaruh terhadap proses - proses yang terjadi di pantai terutama gelombang dan arus bergantung pada bentuk dan karakteristik pantai. Hidrodinamika merupakan sebuah konsep sistem model numerik secara umum untuk memodelkan suatu simulasi baik simulasi muka air, aliran di estuari, teluk dan pantai. 
* Sedangkan Hidrodinamika 1D merupakan model untuk mensimulasikan pola gerak dari air laut secara global dengan satu variabel (x saja atau y saja)

Pemodelan Hidrodinamika 1 Dimensi :
- Model Hidrodinamika 1D lebih cocok diterapkan pada gradien (kemiringan lereng) rendah atau cenderung landai
- Memiliki model elevasi muka air yang seragam di seluruh penampang dan tidak dipengaruhi oleh kedalaman
- Daerah yang direpserentasikan diambil tegak lurus terhadap aliran dan mewakili 1 sumbu (x atau y)

Persamaan utama:
- Persamaan Momentum
Persamaan Momentum 1 Dimensi Sederhana dapat ditulis
<img width="117" alt="Screen Shot 2022-05-21 at 17 21 29" src="https://user-images.githubusercontent.com/105969814/169647277-aa024355-beb3-40a4-9ed4-be647fe03a78.png">
Arti fisis : “Adanya pergerakan air atau arus yang diakibatkan oleh perubahan elevasi terhadap tuang atau adanya gradient elevasi”.

- Persamaan Kontinuitas 
Persamaan Kontinuitas 1 Dimensi Sederhana dapat ditulis
<img width="134" alt="Screen Shot 2022-05-21 at 17 21 09" src="https://user-images.githubusercontent.com/105969814/169647262-f39f6d47-7dde-41fb-8809-f387773ae7c2.png">
Arti fisis :”Perubahan elevasi terhadap waktu diakibatkan adanya perubahan kecepatan terhadap waktu”

# Langkah pengerjaan Script Hidrodinamika 1D
1. Pilih satu aplikasi untuk menjalankan script ini seperti Jupyter Notebook, Visual Studio Code atau Google Colaboratory. Kemudian meng-import mandatory library berupa matplotlib.pyplot (plt) dan numpy (np). Dilengkapi juga dengan pendefinisian model yang akan dijalankan.
# Modul Hidrodinamika 2 Dimensi
- Pengertian dan Persamaan Pembangun
* Hidrodinamika 2D merupakan
