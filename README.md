Portofolio Minimal Futuristik
Sebuah website portofolio pribadi modern bergaya brutalist yang dibangun menggunakan Next.js (App Router), Tailwind CSS, dan TypeScript.
Fitur
Desain Futuristik: Estetika bersih, gelap, dan kuat dengan aksen warna ungu.
Manajemen Proyek: Panel admin untuk mengelola proyek.
CMS Berbasis File: Data proyek disimpan di src/data/projects.json.
Integrasi GitHub: Mempublikasikan pembaruan langsung ke GitHub untuk memicu deployment otomatis di Vercel.
Autentikasi: Akses admin berbasis kata sandi sederhana.
Teknologi yang Digunakan
Next.js 16 (App Router)
Tailwind CSS 4
TypeScript
Framer Motion
Lucide React
Octokit (GitHub API)
Jose (Autentikasi JWT)
Instalasi
Clone repository:
Bash
Salin kode
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Install dependencies:
Bash
Salin kode
npm install
Konfigurasi Environment Variables: Salin file .env.example menjadi .env.local, lalu isi nilainya:
Bash
Salin kode
cp .env.example .env.local
ADMIN_PASSWORD: Kata sandi untuk mengakses panel admin.
JWT_SECRET: Kunci rahasia untuk menandatangani JWT. Gunakan string acak yang kuat.
GITHUB_TOKEN: GitHub Personal Access Token (PAT) dengan izin repo.
GITHUB_REPO_OWNER: Username GitHub Anda.
GITHUB_REPO_NAME: Nama repository ini.
Menjalankan secara lokal:
Bash
Salin kode
npm run dev
Buka http://localhost:3000 untuk melihat website publik.
Buka http://localhost:3000/admin untuk mengakses panel admin.
Deployment di Vercel
Push kode Anda ke repository GitHub.
Import proyek tersebut ke Vercel.
Tambahkan semua environment variables dari .env.local ke pengaturan proyek di Vercel.
Lakukan deployment.
Penggunaan Panel Admin
Akses halaman /admin.
Login menggunakan ADMIN_PASSWORD.
Tambahkan atau edit proyek.
Klik "Publish to GitHub" untuk melakukan commit perubahan pada src/data/projects.json.
Tunggu hingga Vercel melakukan redeploy dengan konten terbaru.
Lisensi
MIT