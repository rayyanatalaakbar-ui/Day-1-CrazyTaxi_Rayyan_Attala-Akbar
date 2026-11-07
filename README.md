# Day-1-CrazyTaxi_Rayyan_Attala-Akbar

## 👤 Identitas Peserta

| | |
|---|---|
| **Nama Lengkap** | Rayyan Attala Akbar |
| **Kelompok** | CrazyTaxi_07 |
| **GitHub** | [@rayyanatalaakbar-ui](https://github.com/rayyanatalaakbar-ui) |

---

## Deskripsi Repository

Repository ini berisi dokumentasi kegiatan **Workshop Day 1: "From AI to GitHub – Building with AI, Managing Change with GitHub"** yang dibawakan oleh Nugi Farhan (Senior Product Designer). Isinya mencakup rangkuman materi, poin penting yang saya pelajari, serta pendapat pribadi saya tentang Day 1 Proyek Workshop.

## Tujuan Repository

- Memenuhi tugas dokumentasi Day 1 workshop.
- Menjadi catatan belajar pribadi tentang prompt engineering, Git, dan GitHub.
- Menjadi latihan langsung membuat repository, melakukan commit, dan push ke GitHub.

##  Kegiatan Workshop yang Didokumentasikan

Kegiatan yang didokumentasikan adalah **Workshop Day 1**, dengan dua topik utama:

1. **Membuat dan mengembangkan** dengan bantuan AI (Prompt Engineering).
2. **Manajemen perubahan dan kolaborasi** dengan Git & GitHub.

Proyek yang dikerjakan pada sesi ini adalah **Student Task Planner**, sebuah aplikasi web sederhana untuk mencatat tugas dan deadline mahasiswa.

---

##  Rangkuman Materi Workshop

### 1. Tujuan Pembelajaran Hari Ini
- Menjelaskan bagaimana prompt AI yang lebih spesifik menghasilkan hasil yang lebih baik.
- Mengidentifikasi *repository*, *commit*, *branch*, dan *pull request*.
- Membedakan Git dan GitHub.
- Melakukan *version controlling*.

### 2. Prompt Engineering
**Prompt** adalah instruksi atau masukan yang diberikan kepada model AI untuk mendapatkan hasil tertentu. Bentuknya bisa berupa pertanyaan sederhana, kata kunci, instruksi yang rumit, atau potongan kode. **Prompt engineering** adalah cara merancang instruksi agar AI memberikan jawaban yang tepat, relevan, dan layak digunakan.

**Context is key.** Prompt tanpa konteks (misalnya "Create student task planner") menghasilkan jawaban yang umum dan sulit ditebak. Prompt dengan konteks yang jelas menghasilkan output yang jauh lebih sesuai kebutuhan.

**Struktur prompt yang baik:**

| Komponen | Fungsi |
|---|---|
| **Role** | Menetapkan peran/posisi AI dalam membantu kita |
| **Task** | Menjelaskan tujuan atau tugas utama |
| **Context** | Kebutuhan (*requirements*) dan batasan (*constraints*) |
| **Format** | Bentuk output yang diinginkan |

**Taktik tambahan:** gunakan kata kerja yang jelas, tentukan panjang dan format output, tentukan target audiens, sertakan fakta dan data yang relevan, rujuk sumber atau dokumen tertentu, serta definisikan istilah kunci.

**Keuntungan prompt engineering:**
- Meningkatkan performa model AI
- Mengurangi bias dan respons yang offensive
- Meningkatkan kontrol dan *predictability*
- Memberikan pengalaman yang lebih baik

### 3. Git
**Git** adalah *distributed version control system* (DVCS) yang melacak siapa, kapan, dan apa saja yang diubah dalam suatu file. Git dibuat oleh Linus Torvalds pada tahun 2005.

**Tiga area kerja Git:**
- **Working directory**: salinan satu versi proyek yang sedang dikerjakan.
- **Staging area (index)**: tempat menyimpan informasi perubahan yang akan masuk ke commit berikutnya.
- **Git directory (repository)**: tempat Git menyimpan metadata dan object database proyek.

### 4. Git vs GitHub

| Git | GitHub |
|---|---|
| Sistem version control terdistribusi untuk melacak dan mengelola perubahan kode **secara lokal** | Platform berbasis web untuk menyimpan repository Git **secara online** dan mendukung kolaborasi |

### 5. Perintah Git yang Dipelajari

```bash
# Setup awal
git --version
git config --global user.name "Nama Kamu"
git config --global user.email "email@example.com"
git config --global --list

# Memulai repository
git init                     # memulai repo baru
git clone "url"              # menyalin repo dari GitHub

# Menyimpan perubahan
git add .                    # memindahkan file ke staging area
git add -A                   # sama seperti --all
git commit -m "pesan"        # menyimpan perubahan ke repository

# Terhubung ke GitHub
git remote add origin <url>  # menghubungkan repo lokal ke remote
git push origin main         # mengirim perubahan ke GitHub
git pull origin main         # mengambil dan menggabungkan perubahan
```

### 6. Setup SSH Key
```bash
ssh-keygen -t ed25519 -C "email@domain.com"   # membuat SSH key
ssh -T git@github.com                         # verifikasi koneksi ke GitHub
```
Public key (`id_ed25519.pub`) ditambahkan di **GitHub → Settings → SSH and GPG keys → New SSH key**.

### 7. Alur Praktik Day 1
1. Install platform AI (Claude, Antigravity, ChatGPT)
2. Tulis prompt untuk membuat web/aplikasi
3. Tambahkan ke Git dengan `git init`
4. Commit dan push ke GitHub
5. Lakukan perubahan
6. Commit dan push lagi ke GitHub

---

##  Poin Penting & Pengetahuan Baru

1. **Kualitas output AI bergantung pada kualitas prompt.** Struktur Role, Task, Context, dan Format membantu prompt jadi jelas dan terarah.
2. **Constraint dan instruksi verifikasi itu penting**, misalnya membatasi teknologi yang dipakai dan meminta AI tidak mengklaim berhasil sebelum diverifikasi.
3. **Git dan GitHub itu berbeda.** Git bekerja secara lokal, GitHub adalah layanan online untuk menyimpan dan berkolaborasi.
4. **Alur dasar Git:** working directory → staging area (`git add`) → repository (`git commit`) → GitHub (`git push`).
5. **Commit message yang jelas** memudahkan melacak riwayat perubahan.
6. **SSH key** membuat koneksi ke GitHub lebih aman dan praktis karena tidak perlu memasukkan password setiap kali push.
7. Prompt yang spesifik dan terstruktur bisa langsung menghasilkan aplikasi sederhana yang siap dikembangkan.

---

## Pendapat Pribadi tentang Day 1 Proyek Workshop

Menurut saya, Day 1 Proyek Workshop sangat bermanfaat karena materinya langsung dipraktikkan. Saya jadi paham bahwa AI bukan sekadar alat "tanya-jawab", tetapi hasilnya sangat dipengaruhi cara kita menulis prompt. Membuat Student Task Planner dengan prompt yang terstruktur memperlihatkan perbedaan nyata dibanding prompt yang singkat.

Di sisi Git dan GitHub, bagian yang paling menantang bagi saya adalah membuat dan menghubungkan repository ke GitHub, tetapi setelah berhasil terasa sangat berguna. Saya jadi memahami pentingnya version control agar setiap perubahan tercatat dan bisa dikelola dengan rapi.

Harapan saya ke depan, sesi berikutnya bisa membahas *branch* dan *pull request* lebih dalam, serta praktik kolaborasi dalam kelompok.

---

*Dibuat oleh Rayyan Attala Akbar — Workshop Day 1, "From AI to GitHub".*
