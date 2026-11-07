# Dokumentasi Workshop: Building with AI & Managing Change with GitHub

Repositori ini dibuat untuk mendokumentasikan proses pembelajaran dan praktik harian dalam sesi workshop mengenai pemanfaatan kecerdasan buatan (*AI*) untuk pengembangan perangkat lunak serta manajemen kontrol versi menggunakan *Git* dan *GitHub*.

---

## 👤 Informasi Peserta
* **Nama Lengkap:** Virdo Zuancarlo Sebastian Sirait
* **Program Studi & Kelas:** TMJ 1C

---

## 🚀 Deskripsi & Tujuan Repository
* **Deskripsi Singkat:** Repositori ini berisi catatan materi, hasil eksplorasi prompt engineering, serta implementasi proyek sederhana berupa *Student Task Planner* berbasis web (*HTML, CSS, JavaScript*) yang dikembangkan dengan bantuan AI dan dikelola melalui *Git version control*.
* **Tujuan Repositori:** Memenuhi penugasan workshop, melatih pemahaman teknis terkait alur kerja *Git* (dari *Working Directory*, *Staging Area*, hingga *Repository*), serta menguji integrasi antara kode lokal dan *remote repository* di GitHub menggunakan autentikasi *SSH Key*.

---

## 📚 Rangkuman Materi Workshop (Day 1)

Berikut adalah ringkasan inti materi yang disampaikan selama sesi workshop:

### 1. Prompt Engineering yang Efektif
* **Definisi:** Prompt adalah instruksi atau masukan yang diberikan kepada model AI untuk menghasilkan output yang spesifik, relevan, dan fungsional[cite: 7].
* **Struktur Prompt yang Baik (R-T-C-F):**
  * **Role:** Menentukan peran AI (contoh: bertindak sebagai *expert web developer*)[cite: 10].
  * **Task:** Menjelaskan tugas utama secara jelas (contoh: membuat aplikasi *Student Task Planner*)[cite: 10].
  * **Context:** Memberikan latar belakang dan kebutuhan spesifik proyek[cite: 10].
  * **Constraints & Format:** Menentukan batasan teknologi (misal: hanya pakai *vanilla JavaScript* tanpa library tambahan) serta format output yang diinginkan[cite: 10].

### 2. Git vs GitHub
* **Git:** Sistem *Version Control* terdistribusi (DVCS) yang berjalan secara lokal di komputer untuk melacak setiap perubahan riwayat kode, diciptakan oleh Linus Torvalds pada tahun 2005[cite: 15, 17].
* **GitHub:** Platform berbasis web untuk menyimpan repositori Git secara *online* serta memfasilitasi kolaborasi tim secara global[cite: 17].

### 3. Alur Kerja Git (*Git Workflow*)
* **Working Directory:** Salinan file proyek fisik yang sedang kita modifikasi di komputer[cite: 16].
* **Staging Area (Index):** Ruang transisi untuk menyiapkan dan mendaftarkan file apa saja yang akan disertakan dalam *commit* berikutnya[cite: 16].
* **Git Directory (.git):** Tempat penyimpanan *metadata* dan basis data objek proyek secara lokal[cite: 16].

### 4. Perintah Dasar Git & GitHub (*Essential Commands*)
* `git init`: Memulai atau menginisialisasi repositori Git baru[cite: 18].
* `git add .` / `git add --all`: Memindahkan perubahan file dari *working directory* ke *staging area*[cite: 18, 23].
* `git commit -m "pesan"`: Menyimpan snapshot perubahan permanen ke dalam riwayat repositori lokal[cite: 18].
* `git remote add origin <url>`: Menghubungkan repositori lokal dengan *remote repository* di GitHub.
* `git push origin main`: Mengunggah (*push*) *branch* utama beserta riwayat perubahannya ke GitHub[cite: 19].
* `git pull origin main`: Mengambil dan menggabungkan pembaruan dari *remote repository* ke lingkungan kerja lokal[cite: 19].

---

## 💡 Poin-Poin Penting & Pengetahuan Baru

* **Pentingnya Konteks dalam AI:** Memberikan instruksi mentah tanpa konteks sering kali membuahkan hasil yang kurang akurat. Dengan menerapkan struktur *Role, Task, Context, Format*, AI dapat menghasilkan kode program yang bersih, terstruktur, dan minim eror.
* **Keamanan Akses via SSH Key:** Mempelajari pembuatan kunci kriptografi berbasis *Ed25519* (`ssh-keygen -t ed25519`)[cite: 24] untuk mengamankan komunikasi autentikasi antara perangkat lokal dan GitHub tanpa harus selalu memasukkan kata sandi manual.
* **Disiplin State Management:** Memahami bahwa perubahan sekecil apa pun pada kode harus melalui siklus logis (*Edit ➔ Add ➔ Commit ➔ Push*) agar riwayat pengembangan proyek tercatat rapi dan profesional.

---

## 💭 Pendapat Pribadi tentang Proyek Day 1

> Sesi *Day 1* ini memberikan sudut pandang yang sangat menarik mengenai bagaimana seorang developer modern bekerja. Menggabungkan kecepatan eksplorasi logika melalui AI dengan kontrol versi yang presisi menggunakan Git membuat proses pembuatan aplikasi menjadi jauh lebih terstruktur. Tantangan utamanya bukan lagi sekadar mengetik kode dari nol, melainkan bagaimana kita bisa merancang perintah (*prompt*) yang presisi dan menjaga kerapian repositori agar mudah dikelola, dipahami oleh tim lain, serta siap dikembangkan ke skala yang lebih besar.
