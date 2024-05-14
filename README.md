#  09 | Setup Database dan Fetching Data

## Praktikum 1: Setup Database

**Membuat project baru dengan template**

1. Mulailah membuat repo berdasarkan templat starter code ini: https://github.com/jti-polinema/09-nextjs-database (klik pada Use this template) kemudian beri nama repo: 09-nextjs-database pada akun GitHub Anda.

**Membuat Akun Vercel**

2. Selanjutnya buat akun vercel (jika Anda belum memilikinya) di tautan ini https://vercel.com/signup
3. Pilih **plan free "hobby"** dan isi dengan nama Anda.
4. Kemudian pilih **Continue with GitHub** untuk terkoneksi dengan akun Vercel.

**Koneksikan dan Deploy project Anda**

5. Selanjutnya, Anda akan diarahkan screen berikut untuk memilih repo dan impor dari GitHub yang telah Anda buat pada langkah nomor 1 tadi.
6. Beri nama project Anda dan klik Deploy.
7. Tunggu proses deploy selama ± 1 menit.
8. Hooray! 🥳 Project Anda sekarang sudah berhasil deploy di server Vercel.

> **Soal 1**
>
> Capture hasil deploy project Anda dan buatlah laporan di file README.md. Jelaskan apa yang telah Anda pelajari?
>
> Jangan lupa push dengan pesan commit: `"W09: Jawaban soal 1"`.

![Output](img/ss1.png)

**Membuat basis data Postgres**

1. Selanjutnya untuk setup database, klik **Continue to Dashboard** dan pilih tab **Storage** pada dashboard project Anda. Lalu pilih **Create** pada basis data **Postgres**.
2. Setujui terms, beri nama basis data, dan pastikan region basis data di set ke **Washington D.C (iad1)** - ini merupakan default region untuk semua project baru di Vercel. Meletakkan basis data pada region yang sama atau semakin dekat dengan kode aplikasi, Anda dapat mengurangi latency pada tiap request data.
3. Setelah berhasil terhubung, arahkan pada tab `.env.local`, klik **Show secret** dan **Copy Snippet** seperti pada gambar berikut.
4. Buat file baru `.env` pada root project Anda, lalu **paste** hasil **Copy Snippet** tersebut.

>**Penting**: Buka file `.gitignore` dan pastikan file `.env` tercantum didalamnya agar konfigurasi rahasia basis data tidak terekspos ketika melakukan push ke GitHub.

5. Akhirnya, jalankan perintah berikut di terminal untuk install Vercel Postgres SDK.
```
npm i --save @vercel/postgres
```

> **Soal 2**
>
> Capture hasil deploy project Anda dan buatlah laporan di file README.md. Jelaskan apa yang telah Anda pelajari?
>
> Jangan lupa push dengan pesan commit: `"W09: Jawaban soal 2"`.

Jawab: Selain dalam hal deployment proyek dari Github, Vercel juga dapat membantu dalam pembuatan Database, pada praktikum ini dilakukan pembuatan database Postgres dengan Vercel, untuk mengakses Database ini maka perlu dibuat file .env dan menambahkan file tersebut ke .gitignore agar kode untuk akses database tersebut tidak ikut terpush ke Github.

![Output](img/ss2.png)