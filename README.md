# Final Pemrograman Web Lanjut 20241

## Anggota Kelompok

| Nama               | NIM          |
| ------------------ | ------------ |
| HAMDANI            | 105841103722 |
| FAJAR EKA ALAMSYAH | 105841100332 |
| KHOIRUL UMAM       | 105841100221 |
| NUR MILANI HIDAYAH | 105841100822 |
| SYARIPUDDIN        | 105841101222 |
| FAJAR RAHMAH       | 105841102022 |




## 📂 Struktur Folder

### Backend (NestJS)
```
📂 BACK-END
├── 📁 dist/                 # Folder hasil build (dihasilkan setelah build dengan TypeScript)
├── 📁 node_modules/         # Folder dependencies yang diinstal oleh npm/yarn
├── 📁 prisma/               # Folder untuk konfigurasi Prisma ORM
├── 📁 src/                  # Folder utama yang berisi source code aplikasi
│   ├── 📁 dto/              # Data Transfer Objects (DTO) untuk validasi dan struktur data
│   ├── 📁 entity/           # Definisi entity sesuai dengan database
│   ├── 📁 shared/           # Helper atau utilitas yang dapat digunakan di seluruh aplikasi
│   ├── 📄 app.controller.spec.ts # Unit testing untuk AppController
│   ├── 📄 app.controller.ts      # Controller utama yang menangani HTTP request
│   ├── 📄 app.module.ts          # Modul utama aplikasi
│   ├── 📄 app.service.ts         # Service utama untuk logika bisnis
│   ├── 📄 auth.guard.ts          # Guard untuk otentikasi dan otorisasi
│   ├── 📄 auth.module.ts         # Modul untuk autentikasi pengguna
│   ├── 📄 main.ts                # Entry point dari aplikasi (inisialisasi NestJS)
│   ├── 📄 prisma.service.ts      # Service untuk komunikasi dengan database menggunakan Prisma
│   ├── 📄 user.decorator.ts      # Custom decorator untuk pengguna
├── 📁 test/                 # Folder untuk file testing aplikasi
├── 📁 uploads/              # Folder untuk menyimpan file yang diunggah
├── 📄 .env                  # File konfigurasi environment variables
├── 📄 .gitignore            # File untuk menentukan file/folder yang harus diabaikan oleh Git
├── 📄 .prettierrc           # Konfigurasi Prettier untuk format kode
├── 📄 nest-cli.json         # Konfigurasi NestJS CLI
├── 📄 package.json          # Konfigurasi proyek, termasuk dependencies dan scripts
├── 📄 tsconfig.build.json   # Konfigurasi TypeScript khusus untuk proses build
└── 📄 tsconfig.json         # Konfigurasi utama TypeScript
```




### Frontend (ReactJS)

```
📂 FRONTEND
├── 📂 .vscode/                   # Konfigurasi VS Code
├── 📂 node_modules/             # Folder dependencies yang diinstal oleh npm/yarn
├── 📂 public/                   # Folder untuk aset statis (gambar, favicon, dll.)
├── 📂 src/                      # Folder utama yang berisi source code aplikasi
│   ├── 📂 assets/               # Folder untuk menyimpan gambar, ikon, atau aset lainnya
│   ├── 📂 hooks/                # Custom React hooks
│   │   ├── 📄 useFetch.tsx      # Hook untuk fetch API
│   │   ├── 📄 useUser.tsx       # Hook untuk user data
│   ├── 📂 layout/               # Komponen Layout utama aplikasi
│   │   ├── 📄 index.tsx         # Layout utama aplikasi
│   ├── 📂 pages/                # Halaman utama aplikasi
│   │   ├── 📂 home/             
│   │   ├── 📂 login/            
│   │   ├── 📂 logout/           
│   │   ├── 📂 Pengaturan/       
│   │   ├── 📂 Profile/          
│   │   ├── 📂 register/         
│   │   ├── 📂 Tambah_Kehamilan/
│   ├── 📂 utils/                # Helper atau fungsi utilitas
│   ├── 📄 App.css               # File styling utama aplikasi
│   ├── 📄 App.tsx               # Komponen utama aplikasi React
│   ├── 📄 index.css             # Styling global aplikasi
│   ├── 📄 main.tsx              # Entry point aplikasi React
│   ├── 📄 vite-env.d.ts         # Konfigurasi environment untuk Vite
├── 📄 .gitignore                # File untuk menentukan file/folder yang diabaikan oleh Git
├── 📄 eslint.config.js          # Konfigurasi ESLint
├── 📄 index.html                # File HTML utama aplikasi
├── 📄 package.json              # Konfigurasi proyek, dependencies, dan scripts
├── 📄 package-lock.json         # Lock file untuk dependencies
├── 📄 README.md                 # Dokumentasi proyek
├── 📄 tsconfig.app.json         # Konfigurasi TypeScript untuk aplikasi
├── 📄 tsconfig.json             # Konfigurasi utama TypeScript
├── 📄 tsconfig.node.json        # Konfigurasi TypeScript untuk Node
├── 📄 vite.config.ts            # Konfigurasi Vite untuk build dan development
```



## Instalasi dan Menjalankan Aplikasi

### Backend (NestJS)

1. Pastikan Node.js sudah terinstal

   - Download dari [Node.js Official Website](https://nodejs.org/)

2. Install NestJS CLI

   ```sh
   npm install -g @nestjs/cli
   ```

3. Clone repository backend

   ```sh
   git clone https://github.com/hamdani105841103722/BACKEND.git
   cd BACKEND
   ```

4. Install dependencies

   ```sh
   yarn install
   ```

5. Generate Prisma

   ```sh
   npx prisma generate
   ```

6. Jalankan backend

   ```sh
   yarn run start:dev
   ```

### Frontend (ReactJS)

1. Clone repository frontend

   ```sh
   git clone [URL REPOSITORY FRONTEND]
   cd FRONTEND
   ```

2. Install dependencies

   ```sh
   yarn install
   ```

3. Jalankan frontend

   ```sh
   yarn run dev
   ```

## Akses Aplikasi

- Backend: (https://automatic-cod-wr7rp75p997wc57q7-3000.app.github.dev/api)
- Frontend: (https://super-spork-5gqgjqrjvw642vxpr-5173.app.github.dev/login)

( Jika Ingin Mengakses, Pastikan BACKEND Atau FRONTEND Berjalan)

## Troubleshooting

Jika mengalami error:

1. Pastikan semua dependencies telah terinstall dengan `yarn install`.
2. Pastikan database telah dikonfigurasi dengan benar di `.env`.
3. Jalankan ulang dengan perintah berikut:
   ```sh
   yarn run start:dev
   ```

## Menjalankan Program BACKEND dan FRONTEND di Dalam Codespaces

1. Jalankan Backend

   ```sh
   1. cd BACKEND
   2. yarn run start:dev
   ```

2. Jalankan Frontend di Terminal Baru

   ```sh
   1. cd FRONTEND
   2. yarn run dev
   ```
   
3. Jika Sudah Menjalankan Frontend Maka Akan Muncul Sebuah Localhost dan Silahkan Klik Link Tersebut
   ```sh
   http://localhost:5173/
   ```
4. Jika Terjadi Error, Lihat Kembali Bagian Troubleshooting

## Akun untuk Login

Karena tidak ada menu registrasi di frontend, gunakan akun berikut untuk login:

- **Username:** Kelompok1
- **Password:** unismuh123

## Akses Project Backend

Backend tidak disertakan dalam repository ini. Untuk mengakses backend, gunakan link berikut:
[https://github.com/hamdani105841103722/BACKEND.git](https://github.com/hamdani105841103722/BACKEND.git)

## Catatan

Jika masih mengalami error, coba jalankan ulang perintah berikut:

```sh
yarn install
yarn add @nestjs/common @nestjs/core typescript --save
npx prisma generate
yarn run start:dev
```

Sekian Assalamualaikum Warahmatullahi Wabarakatuh

