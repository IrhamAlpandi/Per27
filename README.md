A.	PRAKTIKUM I
1.	Kita buat project baru dengan mengetik perintah berikut pada Terminal atau CMD composer create-project laravel/laravel:^10.0 laravel-auth-app
 ![image](https://github.com/user-attachments/assets/06c5dcd1-cdd1-4308-8b48-45492fb3665d)

2.	Kemudian kita modifikasi file .env agar dapat terkoneksi dengan SQLite seperti berikut.
 ![image](https://github.com/user-attachments/assets/080e0756-7533-4816-99dc-4e44cc7c424b)

3.	Setelah selesai, selanjutnya kita lakukan migrate dengan perintah berikut php artisan migrate 
 ![image](https://github.com/user-attachments/assets/1cfc29f5-4e91-4e90-a0cb-2ba113ae06aa)

4.	Sekarang kita unduh starter kit breeze dengan composer melalui perintah berikut composer require laravel/breeze --dev 
 ![image](https://github.com/user-attachments/assets/2d1a853d-3851-4b25-a9b2-f01c7c23f712)

5.	Kemudian install dengan perintah artisan berikut php artisan breeze:install Proses instalasi seperti gambar berikut
 ![image](https://github.com/user-attachments/assets/d60f92d6-38c1-4901-b0f1-e816f31579ae)

6.	Selanjutnya jalankan perintah berikut
 ![image](https://github.com/user-attachments/assets/9935eb40-cd64-4edf-94f9-05cf083050d7)

7.	Selanjutnya, kita run dengan perintah php artisan serve lalu hasilnya seperti gambar berikut. Perhatikan di pojok kanan atas, terdapat menu untuk Log in dan Register.
 ![image](https://github.com/user-attachments/assets/27211667-572f-4a4e-a7ef-191e95ae4528)

B.	PRAKTIKUM II
1.	Kita akan menggunakan Laravel Blog Starter Kit yang dibangun dengan Laravel 10, Tailwind CSS, AlpineJS, dan Livewire.
2.	Lakukan git clone dengan perintah berikut di Terminal 
git clone https://github.com/jti-polinema/laravel-blogkit 
 ![image](https://github.com/user-attachments/assets/ca63c128-5254-4ac4-8e83-4b987ab64498)

3.	Kemudian buka project laravel-blogkit dengan code editor favorit Anda, lalu install dependensi dengan perintah composer install
 ![image](https://github.com/user-attachments/assets/ab99e24c-1c33-4a74-8cae-21e2fd6cd6c3)

4.	Pada bagian config file config/blog.php ubahlah demoMode menjadi true 
 ![image](https://github.com/user-attachments/assets/a0fac25a-91e1-455a-b8f0-5843c4e22908)

5.	Lalu rename file .env.example menjadi .env 
6.	Sesuaikan DB config dengan menggunakan SQLite seperti pada praktikum 1 sebelumnya. 
 ![image](https://github.com/user-attachments/assets/1e3bc52c-dce3-490c-9da1-0d8dcda85ff9)

7.	Kemudian jalankan perintah berikut untuk menggenerate key pada .env 
php artisan key:generate 
 ![image](https://github.com/user-attachments/assets/0448240c-ad0f-4027-9f1e-f1f8bc078795)

8.	Lalu lakukan migration dengan perintah berikut php artisan migrate 
 ![image](https://github.com/user-attachments/assets/e7d14b0c-546c-4893-8516-8948a3b5a18c)

9.	Selanjutnya kita buat akun admin dengan cara menjalankan perintah berikut php artisan admin:create 
 ![image](https://github.com/user-attachments/assets/50c182e8-08bb-45eb-937a-2b80f82fb644)

Hasilnya seperti gambar berikut Terakhir coba running dengan perintah php artisan serve 
 ![image](https://github.com/user-attachments/assets/a0cbd22e-75ae-4892-b407-3e53593602a4)

10.	Coba login dengan akun admin, pelajari setiap menu dan tampilan yang ada. 
 
11.	Buatlah akun dengan cara register, lalu ubah otorisasi antara admin, guest, author, dan akun yang diblokir (banned).
