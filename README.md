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

- Dalam pemrograman Adveksi-Difusi 2 Dimensi, dibutuhkan 3 library, yaitu matplotlib, numpy, dan sys. Matplotlib berfungsi untuk membuat plot grafik dari hasil running. Numpy berfungsi untuk menyimpan data sebagai grid atau matriks. Sys berfungsi untuk mengakses konfigurasi interpreter pada saat runtime dan berinteraksi dengan environment sistem operasi.
- Dari hasil pemodelan yang dikerjakan, dapat terlihat bahwa awalnya polutan awalnya hanya berada di 1 titik dan konsentrasinya sangat pekat. Seiring berjalannya waktu, polutan menyebar dan bergerak ke arah theta diikuti dengan menurunnya konsentrasi polutan tersebut.
- Persamaan Adveksi-Difusi terutama 2 Dimensi adalah persamaan matematis yang didesain untuk mempelajari fenomena transpor polutan. Persamaan ini menggambarkan model pemodelan oseanografi yang menggambarkan proses transportasi suatu zat yang dipengaruhi gaya dalam dua dimensi.
- Penerapan Adveksi-Difusi 2 Dimensi dalam bidang oseanografi, antara lain: memprediksi penyebaran polutan di perairan, memprediksi penyebaran nutrien di perairan.
# Langkah pengerjaan Script Adveksi-Difusi 2D
1. Pilih satu aplikasi untuk menjalankan script ini seperti Jupyter Notebook, Visual Studio Code atau Google Colaboratory. Kemudian meng-import mandatory library berupa matplotlib.pyplot, numpy dan sys. Dilengkapi juga dengan pendefinisian model yang akan dijalankan.
  <img width="223" alt="image" src="https://user-images.githubusercontent.com/105967772/169658150-53160ec0-08f5-440d-a46e-5fdabaa70e1b.png">

    
2. Selanjutnya dimasukkan parameter awal dan parameter lanjutan untuk perhitungan polutan yang akan digunakan.
  <img width="160" alt="image" src="https://user-images.githubusercontent.com/105967772/169657797-b43f9b2b-b001-4000-a76b-8f95a2a20674.png">



3. Setelah itu dilakukan perhitungan dibuat dengan rumusan U dan V untuk mengetahui sebaran dari polutan.
  <img width="375" alt="image" src="https://user-images.githubusercontent.com/105967772/169657815-9b0f07d2-d4f5-4346-aea6-c8b3f45c19b4.png">
  <img width="306" alt="image" src="https://user-images.githubusercontent.com/105967772/169658203-dc72b21b-2b54-4ae4-9634-5040384e982a.png">



4. Dilanjutkan dengan pembuatan grid agar dalam pembuatan model sebagai boundary atau batas alat bantu untuk menyusun dan mengatur hasil akhir sebaran polutan.
  <img width="279" alt="image" src="https://user-images.githubusercontent.com/105967772/169657843-dba77d24-62f5-4c90-a590-30a7c6995d09.png">


5. Dilakukan iterasi otomatis sampai memenuhi syarat batas kestabilan.
  <img width="613" alt="image" src="https://user-images.githubusercontent.com/105967772/169657897-d3639d30-357f-483e-bc7b-a5ea80066346.png">


6. Langkah terakhir yaitu membuat script untuk labelling pada grafik output sebaran polutan.
  <img width="434" alt="image" src="https://user-images.githubusercontent.com/105967772/169657924-35d7869c-9b0e-43ef-bf13-8ba894cd8b5d.png">


7. Script siap dijalankan

# Modul Hidrodinamika 1 Dimensi
- Pengertian dan Persamaan Pembangun
Pada persamaan hidrodinamika 1 dimensi sederhana persamaan pembangun yang digunakan adalah persamaan kontunuitas dan persamaan momentum atau gerak. Persamaan kontinuitas atau kekelalan massa dimana setiap benda yang masuk dama dengan yang keluar
Momentum merupakan hasil perkalian antara massa dan kecepatan suatu objek. Persamaan momentum didasarkan pada persamaan Hk. II Newton yang berbunyi “setiap benda bermassa yang dikenai gaya akan menimulkan percepatan”. Persamaan Momentum 1 Dimensi Sederhana dapat ditulis:
<img width="125" alt="Screen Shot 2022-05-21 at 17 20 14" src="https://user-images.githubusercontent.com/105969814/169647226-f9265f93-733e-45fd-b973-5e4b68b608ae.png">

* Hidrodinamika merupakan salah satu cabang ilmu pengetahuan yang mempelajari gerak liquid atau gerak fluida cair khususnya gerak air, kondisi hidrodinamika merupakan salah satu aspek yang sangat berpengaruh terhadap proses - proses yang terjadi di pantai terutama gelombang dan arus bergantung pada bentuk dan karakteristik pantai. Hidrodinamika merupakan sebuah konsep sistem model numerik secara umum untuk memodelkan suatu simulasi baik simulasi muka air, aliran di estuari, teluk dan pantai. 
* Sedangkan Hidrodinamika 1D merupakan model untuk mensimulasikan pola gerak dari air laut secara global dengan satu variabel (x saja atau y saja)
* Dalam pemrograman Hidrodinamika 1 Dimensi, dibutuhkan 2 library, yaitu matplotlib dan numpy. Matplotlib berfungsi untuk membuat plot grafik dari hasil running. Numpy berfungsi untuk menyimpan data sebagai grid atau matriks.

Pemodelan Hidrodinamika 1 Dimensi :
- Model Hidrodinamika 1D lebih cocok diterapkan pada gradien (kemiringan lereng) rendah atau cenderung landai
- Memiliki model elevasi muka air yang seragam di seluruh penampang dan tidak dipengaruhi oleh kedalaman
- Daerah yang direpserentasikan diambil tegak lurus terhadap aliran dan mewakili 1 sumbu (x atau y)

Persamaan Utama:
- Persamaan Momentum:
<img width="117" alt="Screen Shot 2022-05-21 at 17 21 29" src="https://user-images.githubusercontent.com/105969814/169647277-aa024355-beb3-40a4-9ed4-be647fe03a78.png">
Arti fisis : “Adanya pergerakan air atau arus yang diakibatkan oleh perubahan elevasi terhadap tuang atau adanya gradient elevasi”

- Persamaan Kontinuitas:
<img width="134" alt="Screen Shot 2022-05-21 at 17 21 09" src="https://user-images.githubusercontent.com/105969814/169647262-f39f6d47-7dde-41fb-8809-f387773ae7c2.png">
Arti fisis :"Perubahan elevasi terhadap waktu diakibatkan adanya perubahan kecepatan terhadap waktu"


- Persamaan Transport:

<img width="200" alt="Screen Shot 2022-05-21 at 17 21 29" src="https://user-images.githubusercontent.com/105966336/169685294-255d7d59-a48c-4acc-a470-2848710d3b3c.png">

Diskritisasi
- CTCS

![Screenshot (485)](https://user-images.githubusercontent.com/105966336/169685325-8859d04d-0e99-4424-bbc3-d35654b2cb75.png)

- FTCS

![Screenshot (484)](https://user-images.githubusercontent.com/105966336/169685332-eeb8f522-fdf6-40cb-be4a-d655275dd27d.png)


Kelemahan Model  Hidrodinamika:
* Banyak Data
* Rawan Error terhadap Perhitungan Kritis (Perhitungan nilai CFL)
* Simulasi Lama (tergantung perangkat/processor)


Penerapan Dalam Bidang Oseanografi
- Mengetahui sebaran tumpahan minyak mentah yang ada di perairan menggunakan data arah pergerakan arus pasang surut
- Untuk mengkaji fenomena suhu dingin di perairan
- Mengetahui sebaran limbah air panas yang masuk ke perairan



# Langkah pengerjaan Script Hidrodinamika 1D
1. Pilih satu aplikasi untuk menjalankan script ini seperti Jupyter Notebook, Visual Studio Code atau Google Colaboratory. Kemudian meng-import mandatory library berupa matplotlib.pyplot (plt) dan numpy (np). Dilengkapi juga dengan pendefinisian model yang akan dijalankan.
```
import matplotlib.pyplot as plt
import numpy as np
```
2. Memasukkan paremeter awal untuk model hidrodinamika.
```
p = 5000 #Panjang Awal
T = 1200 #Waktu Simulasi
A = 0.5 #Amplitudo
D = 15 #Depth/kedalaman
dt = 2
dx = 100
To = 300 #Periode

g = 9.8
pi = np.pi
C = np.sqrt(g*D) #Kecepatan Arus
s = 2*pi/To #Kecepatan Sudut Gelombang
L = C*To #Panjang Gelombang
k = 2*pi/L #Koefisien Panjang Gelombang
Mmax = int(p//dx)
Nmax = int(T//dt)
```

3. Selanjutnya dibuat script phyton untuk pendefenisian persamaan hidrodinamika pada grid.
```
zo = [None for _ in range(Mmax)]
uo = [None for _ in range (Mmax)]

hasilu = [None for _ in range(Nmax)]
hasilz = [None for _ in range (Nmax)]

for i in range(1, Mmax+1):
    zo[i-1] = A*np.cos(k*(i)*dx)
    uo[i-1] = A*C*np.cos(k*((i)*dx+(0.5)*dx))/(D+zo[i-1])
for i in range(1, Nmax+1):
    zb = [None for _ in range(Mmax)]
    ub = [None for _ in range(Mmax)]
    zb[0] = A*np.cos(s*(i)*dt)
    ub[-1] = A*C*np.cos(k*L-s*(i)*dt)/(D+zo[-1])
    for j in range(1, Mmax):
        ub[j-1] = uo[j-1]-g*(dt/dx)*(zo[j]-zo[j-1])
    for k in range(2, Mmax+1):
        zb[k-1] = zo[k-1]-(D+zo[k-1])*(dt/dx)*(ub[k-1]-ub[k-2])
        hasilu[i-1] = ub
        hasilz[i-1] = zb
    for p in range(0, Mmax):
        uo[p] = ub[p]
        zo[p] = zb[p]
```

4. Kemudian dibuat grafik yang memuat pendefenisian-pendefenisian dari persamaan hidrodinamika yang sudah dibuat sebelumnya.
```
def rand_col_hex_string():
    return f'#{format(np.random.randint(0,16777215), "#08x")[2:]}'

hasilu_np = np.array(hasilu)
hasilz_np = np.array(hasilz)

fig0, ax0 = plt.subplots(figsize=(12,8))
for i in range(1, 16):
    col0 = rand_col_hex_string()
    line, = ax0.plot(hasilu_np[:,i-1], c=col0, label=f'n={i}')
    ax0.legend()

    ax0.set(xlabel='Waktu', ylabel='Kecepatan Arus',
            title=''' Nama_NIM
            Perubahan Kecepatan Arus Dalam Grid Tertentu di Sepanjang Waktu''')
    ax0.grid()

fig1, ax1 = plt.subplots(figsize=(12,8))
for i in range(1, 16):
    col1 = rand_col_hex_string()
    line, = ax1.plot(hasilz_np[:,i-1], c=col1, label=f'n={i}')
    ax1.legend()

    ax1.set(xlabel='Waktu', ylabel='Elevasi Muka Air',
            title=''' Nama_NIM
            Perubahan Elevasi Permukaan Air Dalam Grid Tertentu di Sepanjang Waktu''')
    ax1.grid()

fig2, ax2 = plt.subplots(figsize=(12,8))
for i in range(1, 16):
    col2 = rand_col_hex_string()
    line, = ax2.plot(hasilu_np[i-1], c=col2, label=f'n={i}')
    ax2.legend()

    ax2.set(xlabel='Grid', ylabel='Kecepatan Arus',
            title=''' Nama_NIM
            Perubahan Kecepatan Arus Dalam Waktu Tertentu di Sepanjang Grid''')
    ax2.grid()

fig3, ax3 = plt.subplots(figsize=(12,8))
for i in range(1, 16):
    col3 = rand_col_hex_string()
    line, = ax3.plot(hasilz_np[i-1], c=col3, label=f'n={i}')
    ax3.legend()

    ax3.set(xlabel='Grid', ylabel='Elevasi Muka Air',
            title=''' Nama_NIM
            Perubahan Elevasi Permukaan Air Dalam Waktu Tertentu di Sepanjang Grid''')
    ax3.grid()
```

5. Grafik Perubahan Kecepatan Arus Dalam Grid Tertentu di Sepanjang Waktu, Perubahan Elevasi Permukaan Air Dalam Grid Tertentu di Sepanjang Waktu, Perubahan Kecepatan Arus Dalam Waktu Tertentu di Sepanjang Grid dan Perubahan Elevasi Permukaan Air  Dalam Waktu Tertentu di Sepanjang Grid ditampilkan dengan perintah:
```
plt.show()
```

# Modul Hidrodinamika 2 Dimensi
- Hidrodinamika adalah cabang dari mekanika fluida, khususnya zat cair inkrompresibel yang dipengaruhi oleh gaya internal dan eksternal. Gaya-gaya penting dalam hidrodinamika laut adalah gaya gravitasi, gaya gesekan, dan gaya coriolis.
- Dalam pemrograman Hidrodinamika 2 Dimensi, dibutuhkan 2 library, yaitu matplotlib, dan siphon. Matplotlib berfungsi untuk membuat plot grafik dari hasil running. Siphon berfungsi untuk mengunduh data dari layanan data jarak jauh.   
* Studi hidrodinamika 2D salah satunya adalah untuk meninjau gaya pembangkit arus yang disebabkan oleh angin.
# Langkah pengerjaan Script Hidrodinamika 2D
1. Buka software Jupyter Notebook melalui Anaconda Prompt (Miniconda 3). Untuk mengerjakan modul ini, pastikan sudah mengunduh mandatory library Matplotlib dan Siphon.
  <img width="212" alt="image" src="https://user-images.githubusercontent.com/105967772/169658835-6f1e9862-7acb-4753-b100-9f6013ead8b8.png">

3. Ketik script pada Jupyter Notebook. Pada bagian Station Id, ubah script sesuai dengan yang diinginkan. Ubah Nama_NIM_Kelas sesuai dengan milik pribadi.
  <img width="397" alt="image" src="https://user-images.githubusercontent.com/105967772/169659194-1d77b7a4-c6d3-4108-a08c-40be1f5a6824.png">

5. Klik Run kemudian akan muncul hasil pemrograman. Simpan hasil grafik yang didapatkan.
6. Buka website NDBC-NOAA.
  <img width="911" alt="image" src="https://user-images.githubusercontent.com/105967772/169659082-51d8ba10-97b4-47e1-9e46-7c7c6f2f4add.png">

8. Cari Station ID sesuai yang yang telah digunakan pada pemrograman tadi. Kemudian identifikasi lokasi buoy yang digunakan.  
 


