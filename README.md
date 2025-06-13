### TASK-SETUP-ANACONDA-UV
Nama : **Alif Nur Rahman**
No Absen : **10.028.DB2025**
Batch : **10**

## Apa Itu Anaconda dan Conda?

**Anaconda** adalah distribusi open-source untuk bahasa pemrograman Python dan R, yang dirancang untuk komputasi ilmiah, analisis data, dan pembelajaran mesin. Anaconda menyederhanakan manajemen paket dan lingkungan, serta mendukung lebih dari 1.500 paket data science yang siap pakai.  

**Conda** adalah manajer paket dan lingkungan yang disertakan dalam Anaconda. Conda memungkinkan pengguna untuk mengelola paket dan lingkungan secara efisien, menghindari konflik dependensi, dan memastikan konsistensi proyek.

---

## Apa Itu UV?

UV adalah alat manajemen lingkungan Python yang memungkinkan pembuatan, pengelolaan, dan penghapusan lingkungan virtual dengan mudah. Berbeda dengan pip dan virtualenv, UV mengintegrasikan pembuatan lingkungan dan instalasi paket dalam satu perintah, serta menyediakan pengelolaan versi Python secara otomatis.

---

## Mengapa Menggunakan UV?

- **Kecepatan**: Instalasi paket dan resolusi dependensi yang lebih cepat dibandingkan dengan pip dan poetry.
- **Kemudahan Penggunaan**: Perintah yang sederhana dan intuitif untuk pembuatan dan pengelolaan lingkungan.
- **Manajemen Versi Python**: Kemampuan untuk mengelola berbagai versi Python tanpa memerlukan alat tambahan.
- **Isolasi Proyek**: Setiap proyek dapat memiliki lingkungan dan dependensi yang terpisah, menghindari konflik antar proyek.

- ## 🐍 Bagian 1: Instalasi Anaconda

**1. Download Installer Anaconda**
   **Apa**
   File installer untuk memasang Anaconda ke komputer Anda.
   **Kenapa**
   Anaconda menyediakan Python dan paket data science siap pakai dalam satu instalasi.

   Langkah-langkah:
    - Buka https://www.anaconda.com/products/distribution
    - Pilih versi sesuai OS Anda (Windows/macOS/Linux)
    - Klik tombol Download

    ![image](![Cuplikan layar 2025-06-13 232537](https://github.com/user-attachments/assets/f5c3dfcd-edf2-43c3-8f58-b68f235e6167)

  #    Do's:
	- Download dari situs resmi Anaconda
	- Simpan installer di folder yang mudah diakses
#   Don'ts:
	- Jangan download dari sumber tidak resmi
	- Jangan simpan di folder system


**2. Jalankan Installer Anaconda**
**1** Klik dua kali file installer Anaconda yang udah kamu download sebelumnya.

**2** Akan muncul wizard instalasi — tinggal klik “Next” beberapa kali.

 ![image](![Cuplikan layar 2025-06-13 005255](https://github.com/user-attachments/assets/92cbdd93-f644-4c37-a1fd-9923d1018443)

**3** Lalu ketika muncul pilihan, Pilih ini :

 ![image](![Cuplikan layar 2025-06-13 231237](https://github.com/user-attachments/assets/7965fda8-10fd-4960-bfc4-8e7a32f14401)

“Add Anaconda to my PATH environment variable”

Klik Install, lalu tunggu prosesnya selesai. Bisa makan waktu beberapa menit tergantung spek laptop kamu.

# ✅ Do’s (Yang Sebaiknya Dilakukan):
- Gunakan pengaturan default aja kalau kamu nggak yakin mau ubah apa — ini udah paling aman dan direkomendasikan.
- Centang opsi “Add to PATH” kalau kamu pengin bisa akses Anaconda langsung dari Command Prompt atau terminal di mana saja.

# ❌ Don’ts (Yang Sebaiknya Dihindari):
- Jangan instal Anaconda ke folder sistem kayak C:\Windows atau C:\Program Files (x86) — bisa bikin error atau butuh izin admin.
- Jangan klik cancel di tengah proses instalasi, apalagi pas udah jalan setengah. Bisa bikin file jadi setengah jadi dan error pas dijalankan.

## 3. ✅ Verifikasi Anaconda Sudah Terpasang dan Bisa Diakses
# Apa sih maksudnya?
Di sini kita mau cek dulu, apakah Anaconda udah beneran ke-install dan bisa dijalankan lewat terminal atau command prompt. Ibaratnya, ini kayak test drive buat lihat apakah semuanya oke sebelum lanjut ke langkah berikutnya.

**Kenapa** perlu dicek?
Biar kamu **TIDAK** kena masalah di tengah jalan, misalnya conda nggak dikenali atau Python-nya belum aktif. Verifikasi ini bakal kasih tahu apakah semua udah beres atau masih ada yang perlu dibenerkan.

## 🪜 Langkah-langkahnya Gampang Banget:
**1** Buka Command Prompt (klik Start → ketik "cmd" → Enter)

**2** Tekan Enter.

**3** jika muncul sesuatu seperti ini:

 ![image](![Cuplikan layar 2025-06-13 232109](https://github.com/user-attachments/assets/f14c155d-2f60-4c29-8c9a-19e7dbd7cbce)

berarti Anaconda kamu udah sukses ke-install dan siap dipakai! 🎉

# ❗Peringatan: Jika lupa mencentang "Tambahkan ke PATH", Anda harus mengatur PATH secara manual.
Coba restart laptop dulu, terus ulangi langkah di atas.
Kalau tetap nggak muncul, mungkin opsi PATH-nya belum dicentang waktu instalasi. Tapi tenang, masih bisa diatur nanti secara manual.
# ✅ Do’s (Yang Perlu Dilakukan):
- Buka terminal baru dulu (jangan pakai yang lama) setelah instalasi selesai — biar pengaturan PATH yang baru kebaca dengan benar.
- Pastikan perintah jalan tanpa error, dan muncul versi conda — itu tandanya Anaconda udah siap dipakai.
# ❌ Don’ts (Yang Harus Dihindari):
- Jangan cuek kalau ada error atau nggak muncul apa-apa. Itu bisa jadi tanda ada yang salah pas instalasi. Lebih baik dicek sekarang daripada nanti pusing pas lagi butuh.

## 4. 🛠️ Cara Menambahkan Anaconda ke PATH (Biar Bisa Diakses dari Mana Aja)
Kadang setelah instalasi, Anaconda belum otomatis bisa dipanggil dari terminal atau CMD. Nah, di sinilah kita tambahkan sendiri ke PATH, supaya conda dan python bisa langsung dikenali dari mana saja.

# 🪜 Langkah-langkah di Windows:
**1** Tekan Windows + R, ketik sysdm.cpl, tekan Enter.
**2** Buka tab "Advanced", lalu klik tombol "Environment Variables…"
**3** Di bagian bawah (System variables), cari dan klik Path, lalu klik Edit.
**4** Klik New, lalu tambahkan dua baris ini (ganti NAMA_ANDA dengan nama user di laptop kamu):

 ![image](![Cuplikan layar 2025-06-13 234228](https://github.com/user-attachments/assets/c9c6bc1f-248b-49d5-beb1-5c66e89f1aba)

# ✅ Do’s (Yang Sebaiknya Dilakukan):
- Tutup dulu terminal/CMD yang lama, terus buka yang baru setelah kamu ubah PATH — biar setting barunya kebaca dengan benar.
- Kalau masih belum bisa, coba restart laptopnya. Kadang Windows baru ngeh setelah di-restart.
# ❌ Don’ts (Yang Harus Dihindari):
- Jangan asal hapus isi PATH lain — itu bisa bikin program penting lain di laptop kamu jadi nggak jalan.
- Edit variabel lingkungan dengan hati-hati, karena ini menyangkut sistem. Kalau ragu, sebaiknya dicatat dulu isi PATH sebelumnya sebelum mengubah.

## 5. 🛠️ Membuat Lingkungan Conda
📌 Apa itu Lingkungan Conda?
Lingkungan Conda adalah ruang kerja virtual yang terisolasi untuk Python dan paket-paket yang digunakan dalam proyek tertentu.

# ❓ Kenapa Perlu Lingkungan Conda?
-Mencegah konflik versi paket antar proyek
- Memastikan stabilitas dan kompatibilitas
- Memudahkan pengelolaan dependensi
# ✅ Do's (yang sebaiknya dilakukan):
- Beri nama atau lokasi environment yang relevan dengan proyek
- Simpan environment di dalam folder proyek untuk portabilitas
# 🪜 Langkah-langkah Praktis:
- Buka Terminal di VS Code
- Tekan Ctrl + ` (tanda backtick di bawah tombol Esc)
- Jalankan perintah berikut untuk membuat environment:
# conda create -p venv python=3.12

![image](![Cuplikan layar 2025-06-14 000153](https://github.com/user-attachments/assets/ae3d97b9-bca0-4658-ad55-8a72590f5fe3)

# Catatan:

- -p venv artinya membuat environment di folder ./venv dalam proyek kamu
- python=3.12 menentukan versi Python yang digunakan Saat muncul pertanyaan: Proceed ([y]/n)?
# ➡️ Ketik y lalu tekan Enter

 ![image](![Cuplikan layar 2025-06-13 235412](https://github.com/user-attachments/assets/d02f5441-974a-4ad1-aef6-87a3a21766a2)

# Setelah selesai, aktifkan environment dengan:
conda activate ./venv

# Prompt terminal akan berubah menjadi:
(venv) C:\Users\ACER\ghost_intellix>

![image](![Cuplikan layar 2025-06-14 001232](https://github.com/user-attachments/assets/90a7f9c2-4a3a-4257-9b8a-d245058ac3da)

Artinya environment berhasil diaktifkan.

## ⚡ Menginstal UV (Ultra Cepat!)
# Apa sih UV itu?
UV itu alat buat ngatur paket dan lingkungan, kayak pip + venv, tapi kecepatannya ngebut karena dibuat pakai Rust. Cocok banget buat proyek yang punya banyak pustaka (dependensi).

# Kenapa pakai UV?
Karena UV bikin proses install jadi jauh lebih cepat. Apalagi kalau proyek kamu besar, ini hemat waktu banget.

# ✅ do's (Lakukan ini):
Pastikan kamu sudah keluar dari environment Conda dulu sebelum pakai UV (biar gak bentrok).

# ❌ don'ts Jangan lakukan ini:
Jangan pakai UV buat install paket-paket khusus Conda, karena UV jalan pakai pip, bukan conda.

# 🚶‍♂️Langkah-langkah Instalasi UV:
- Pastikan environment Conda udah dinonaktifkan: Ketik dulu:
- **conda deactivate**
Kalau udah, prompt bakal balik ke direktori biasa. 2. Install UV: Ketik di terminal atau CMD:

- **pip install uv**
Tunggu sampai muncul tulisan:

- **Successfully installed uv-0.7.12**
Artinya UV berhasil dipasang 🎉

# 🗂️ Tentang Folder ghost_intellixuv
Nanti kita bakal pakai perintah uv init buat bikin folder baru bernama ghost_intellixuv.

# 📌 Catatan penting:
- Kamu nggak perlu bikin folder itu manual.
- UV akan otomatis bikin folder dan isi dasarnya waktu kamu jalanin uv init.
- Setelah itu, kamu bisa ketik:
- **dir**
- buat lihat apakah folder ghost_intellixuv udah muncul.

## 🧪 Membuat & Mengaktifkan Lingkungan UV
# Apa sih maksudnya?
Lingkungan virtual (virtual environment) itu kayak “dunia kecil” khusus buat proyek kamu. Semua pustaka yang diinstal akan disimpan di situ — jadi nggak nyampur sama proyek lain.

# Kenapa penting?
Biar tiap proyek punya ruang sendiri dan gak bikin konflik, apalagi kalau beda versi pustaka.

# ✅ do's (Lakukan ini):
Aktifkan environment sebelum install paket.

# ❌ don'ts (Jangan lakukan ini):
Jangan utak-atik folder .venv secara manual, biarin UV yang ngurus.

## 🚀 Langkah-langkah Bikin dan Aktifkan Environment
1. Ketik:
uv venv
2. Aktifkan:
.venv\Scripts\activate
Prompt berubah ke (ghost_intellixuv) C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>. 3. Ciri-ciri environment sudah aktif: Prompt di terminal bakal berubah, misalnya jadi:

(ghost_intellixuv) C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>
Nah, kalau udah kayak gitu, berarti kamu siap lanjut install paket dan mulai ngoding! 😎

## 📦 Menginstal Paket dengan UV
# Apa sih ini?
UV itu punya fitur keren buat install paket super cepat lewat perintah mirip pip. Tapi di UV, kita pakenya uv add.

# Kenapa pakai UV?
Karena UV install paketnya kilat banget, terutama kalau paketnya besar kayak pandas, numpy, atau matplotlib. Cocok buat kamu yang gak mau nunggu lama! ⚡

# ✅ do's (Lakukan ini):
Install paket pakai uv add (bukan pip install).

# ❌ don'ts (Jangan lakukan ini):
Jangan campur UV dan pip dalam proyek yang sama, nanti bisa bikin konflik dependensi.

## 🚀 Langkah-langkah Install Paket:
- Pastikan environment kamu aktif dulu (lihat ada tanda (ghost_intellixuv) di terminal). Ketik perintah:
- **uv add pandas**
output seperti

- **conda deactivate**
Kalau udah, prompt bakal balik ke direktori biasa. 2. Install UV: Ketik di terminal atau CMD:

- **pip install uv**
Tunggu sampai muncul tulisan:
  [image](![Cuplikan layar 2025-06-14 003008](https://github.com/user-attachments/assets/38312139-a52c-4dab-9018-84990bbcd21c)

Successfully installed uv-0.7.12
Artinya UV berhasil dipasang 🎉

## 🗂️ Tentang Folder ghost_intellixuv
Nanti kita bakal pakai perintah uv init buat bikin folder baru bernama ghost_intellixuv.

# 📌 Catatan penting:
1. Kamu nggak perlu bikin folder itu manual.
2. UV akan otomatis bikin folder dan isi dasarnya waktu kamu jalanin uv init.
3. Setelah itu, kamu bisa ketik:
- **dir**

## 🧪 Membuat & Mengaktifkan Lingkungan UV
# Apa sih maksudnya?
Lingkungan virtual (virtual environment) itu kayak “dunia kecil” khusus buat proyek kamu. Semua pustaka yang diinstal akan disimpan di situ — jadi nggak nyampur sama proyek lain.

# Kenapa penting?
Biar tiap proyek punya ruang sendiri dan gak bikin konflik, apalagi kalau beda versi pustaka.

# ✅ do's (Lakukan ini):
Aktifkan environment sebelum install paket.

# ❌ don'ts (Jangan lakukan ini):
Jangan utak-atik folder .venv secara manual, biarin UV yang ngurus.

## 🚀 Langkah-langkah Bikin dan Aktifkan Environment
# 1. Ketik:
- **uv venv**
# 2. Aktifkan:
- **.venv\Scripts\activate**
Prompt berubah ke (ghost_intellixuv) C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>. 3. Ciri-ciri environment sudah aktif: Prompt di terminal bakal berubah, misalnya jadi:

(ghost_intellixuv) C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>
Nah, kalau udah kayak gitu, berarti kamu siap lanjut install paket dan mulai ngoding! 😎

📦 Menginstal Paket dengan UV
Apa sih ini?
UV itu punya fitur keren buat install paket super cepat lewat perintah mirip pip. Tapi di UV, kita pakenya uv add.

Kenapa pakai UV?
Karena UV install paketnya kilat banget, terutama kalau paketnya besar kayak pandas, numpy, atau matplotlib. Cocok buat kamu yang gak mau nunggu lama! ⚡

# ✅ do's (Lakukan ini):
Install paket pakai uv add (bukan pip install).

# ❌ don'ts (Jangan lakukan ini):
Jangan campur UV dan pip dalam proyek yang sama, nanti bisa bikin konflik dependensi.
