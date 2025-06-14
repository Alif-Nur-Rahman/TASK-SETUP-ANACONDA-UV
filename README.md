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

![Cuplikan layar 2025-06-13 232537](https://github.com/user-attachments/assets/2a9d92b4-fc6d-47de-8292-25445ac868df)




  #    Do's:
	- Download dari situs resmi Anaconda
	- Simpan installer di folder yang mudah diakses
#   Don'ts:
	- Jangan download dari sumber tidak resmi
	- Jangan simpan di folder system


**2. Jalankan Installer Anaconda**
**1** Klik dua kali file installer Anaconda yang udah kamu download sebelumnya.

**2** Akan muncul wizard instalasi — tinggal klik “Next” beberapa kali.

 ![Cuplikan layar 2025-06-13 005255](https://github.com/user-attachments/assets/b5bf50ad-489d-4dcb-880d-05e0f211d61f)


**3** Lalu ketika muncul pilihan, Pilih ini :

 ![Cuplikan layar 2025-06-13 231237](https://github.com/user-attachments/assets/295ef2ac-9af8-44ac-a814-2e034768edc2)


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

 ![Cuplikan layar 2025-06-13 232109](https://github.com/user-attachments/assets/84a72b7d-f47c-4b89-baa4-b7552902f7bb)


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

 ![Cuplikan layar 2025-06-13 234228](https://github.com/user-attachments/assets/663b5270-73f4-478b-917d-90dc78a0fd49)


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


# Catatan:

- -p venv artinya membuat environment di folder ./venv dalam proyek kamu
- python=3.12 menentukan versi Python yang digunakan Saat muncul pertanyaan: Proceed ([y]/n)?
# ➡️ Ketik y lalu tekan Enter

![Cuplikan layar 2025-06-14 215211](https://github.com/user-attachments/assets/70e4c7ec-454f-403d-af87-80443f0f3c92)


# Setelah selesai, aktifkan environment dengan:
conda activate ./venv

# Prompt terminal akan berubah menjadi:
(venv) C:\Users\User\ghost_intellix>


![Cuplikan layar 2025-06-14 215816](https://github.com/user-attachments/assets/602789b8-1d04-4bd6-b106-e0aaccfc5e22)



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
**uv venv**
2. Aktifkan:
**.venv\Scripts\activate**


Prompt berubah ke (ghost_intellixuv) C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>. 3. Ciri-ciri environment sudah aktif: Prompt di terminal bakal berubah, misalnya jadi:

**(ghost_intellixuv) C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>**

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


![Cuplikan layar 2025-06-14 221640](https://github.com/user-attachments/assets/0fee4d95-2551-43b5-a9d4-f533cfd3d7d3)


# 📝 Catatan Penting:

UV jauh lebih cepat dibanding pip, apalagi kalau kamu install paket yang punya banyak “anak paket” alias dependency tree yang besar — contohnya pandas, scikit-learn, atau tensorflow.

# 💡 Jadi kalau proyekmu makin kompleks, UV justru makin terasa manfaatnya: lebih cepat, lebih efisien, dan tetap rapi..

# 🚶‍♂️Langkah Menonaktifkan:

1. Diterminal, ketik:

**.venv\Scripts\deactivate**

2. Setelah itu, prompt akan berubah kembali seperti semula, misalnya:

**C:\Users\NAMA_ANDA\ghost_intellix\ghost_intellixuv>**

Artinya kamu sudah keluar dari lingkungan virtual UV.

## Daftar Paket yang Direkomendasikan
**Apa: Paket penting untuk Data Science, Machine Learning, dan AI.**

**Kenapa: Memastikan alat yang diperlukan tersedia.**

**Do's: Perbarui versi paket secara berkala.**

**Don'ts: Jangan instal paket yang tidak diperlukan.**


**Langkah-langkah:**

1 Buat requitments.txt:


![Cuplikan layar 2025-06-14 225023](https://github.com/user-attachments/assets/abd04c3f-1047-4e66-8114-63b6723a5959)

2. Instal:
   
*uv add -r requirements.txt*

3. atau

*pip install -r requirements.txt*

**🛠️ Panduan Pemecahan Masalah di Anaconda**

**🔧 Masalah 1: conda Tidak Dikenali di Terminal**

Gejala:

*'conda' is not recognized as an internal or external command*

Penyebab:

*PATH Anaconda belum terdaftar di sistem.*

**Solusi:**
1.Pastikan Anaconda sudah diinstal.
2.Tambahkan PATH secara manual (jika belum otomatis):
3.Buka System Properties → Environment Variables.
4.Di bagian “System variables”, cari Path → klik Edit.
5.Tambahkan jalur berikut:

*C:\Users\ACER\anaconda3*
*C:\Users\ACER\anaconda3\Scripts*

6.Jalankan perintah:

*conda init cmd.exe*
7.Tutup dan buka kembali terminal.

#🔧 Masalah 2: Script execution is disabled (saat aktivasi environment)
Gejala:

*File C:... activate.ps1 cannot be loaded because running scripts is disabled*

**Penyebab:**
PowerShell tidak mengizinkan eksekusi skrip.

**Solusi:**
Jalankan PowerShell sebagai Administrator.

**Ketik:**
*Set-ExecutionPolicy RemoteSigned*
Ketik Y untuk mengonfirmasi.

# Kesimpulan

1. Anaconda = “semua‑dalam‑satu” untuk data science; instal sekali, langsung jalan.

2. Conda = motor di balik Anaconda; andal untuk kelola paket lintas‑bahasa & environment terisolasi.
   
 3.UV = solusi modern yang super cepat & ringan ketika Anda hanya butuh Python wheels dari PyPI.


# Pilihan cepat:

1. Data/ML berat & paket C/CUDA → Conda/Anaconda

2. Proyek Python murni & butuh kecepatan → UV


### Semoga Bermanfaat, Terimakasih...SEE YAAAAAAAAA!!!!!👋👋
