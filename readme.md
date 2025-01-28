# Login and Registration Application

Aplikasi ini menyediakan sistem login dan registrasi dengan dua jenis pengguna: **Admin** dan **User**. Admin memiliki akses penuh untuk mengedit data, sedangkan User memiliki akses terbatas. Setelah registrasi, pengguna akan menerima email konfirmasi sebelum dapat login.

## Teknologi yang Digunakan

- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Frontend**: React.js

## Fitur Utama

1. **Halaman Home**

   - Halaman utama aplikasi dengan informasi umum.
   - Screenshot:

     ![Home Page](/scrinsut/beforelogin.png)
     ![afterlogin](/scrinsut/sudahverifikasih.png)

2. **Halaman Login**

   - Pengguna dapat login menggunakan email dan password yang telah terdaftar.

     ![Login Page](/scrinsut/loginkerja.png)

3. **Halaman Register**

   - Pengguna baru dapat mendaftar dengan mengisi nama, email, dan password.
   - Pengguna baru sebelumm mendaftar akan ada konfirmasi ke email klik kode konfirmasi baru bisa login.

     ![Register Page](/scrinsut/registerconfimasion.png)
     ![Register Page](/scrinsut/verifikasihemail.png)
     ![Register Page](/scrinsut/verifikasih.png)
     -baru bisa login setelah klik kode konfirmasi
     ![Register Page](/scrinsut/verifikasihemail.png)

4. **Halaman Lupa Password**

   - Pengguna dapat mengatur ulang password jika lupa dengan memasukkan email terdaftar dan akn ada kode konfirmasi dengan email.

     ![Forgot Password Page](/scrinsut/resetpassword.png)

5. **Halaman Konfirmasi Email**

   - Setelah registrasi, pengguna harus mengkonfirmasi akun melalui email sebelum dapat login.

     ![Email Confirmation Page](/scrinsut/verifikasih.png)

## Langkah-Langkah Menjalankan Aplikasi

1. **Clone Repository**

   ```bash
   git clone <repository-url>
   cd project-directory
   ```

2. **Install Dependencies**

   ```bash
   # Install backend dependencies
   cd backend
   npm install

   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Konfigurasi Environment Variables**
   Buat file `.env` di direktori `backend` dan tambahkan konfigurasi berikut:

   ```env
   MONGO_URI=mongodb://127.0.0.1:27017/login_app
   PORT=5000
   JWT_SECRET=your_jwt_secret
   EMAIL_HOST=smtp.gmail.com
   EMAIL_USER=your-email@gmail.com
   EMAIL_PASS=your-email-password
   ```

   Buat file `.env` di direktori `frontend` dan tambahkan konfigurasi berikut:

   ```env
   REACT_APP_API_URL=http://localhost:5000
   ```

4. **Jalankan Aplikasi**

   ```bash
   # Jalankan backend
   cd backend
   npm start

   # Jalankan frontend
   cd ../frontend
   npm start
   ```

5. **Akses Aplikasi**
   Buka browser dan akses [http://localhost:3000](http://localhost:3000).

## Struktur Folder

```
/project-directory
|-- /backend
|-- /frontend
|-- /scrinsut
|-- readme.md
```

## Fitur Mendatang

- Reset password menggunakan OTP.
- Peningkatan tampilan antarmuka.
- Penambahan dashboard admin untuk manajemen data pengguna.

---

Dikembangkan oleh **[Nama Anda]**.
