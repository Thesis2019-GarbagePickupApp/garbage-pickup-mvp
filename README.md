# MVP of Garbage Pickup App

- ## UI/UX Design
    - [Design](https://www.figma.com/file/JimYF4Ug6TG4932BxkgoVw/AJS-mobile-proses-(Community)?type=design&node-id=0-1&mode=design&t=b5y3weRFZjjKQJwh-0)

- ## Database Schema
    - [Schema](https://dbdiagram.io/embed/649fab0202bd1c4a5e55430f)

- ## List pages
    - Login
       <!-- TODO: show image design of login page here -->
        Pada halaman ini memiliki 2 opsi untuk login 
       - Akun aplikasi

          Login dengan akun aplikasi yang simaksud disini adalah login dengan akun yang sebelumnya sudah terdaftar pada aplikasi penjemputan sampah, login dengan cara ini dapat menggunakan email/nomor hp dan password dengan request body sebagai berikut :
          ```jsonc
         {
            "phone": "",
            "email": "example@gmail.com", // use one of email/phone
            "password": "example_password"
         } 
          ```
       - Akun Google <!-- TODO: maybe move this to stage registration -->

         Dengan cara kedua ini pengguna dapat masuk ke aplikasi dengan menggunakan akun Google sehingga cara untuk aplikasi lebih mudah karena tersambung dengan akun Google. 
        <!-- TODO: add request body here -->
        
        Jika belum memiliki akun untuk masuk ke aplikasi maka pengguna dapat menuju ke halaman pendaftaran sebelum masuk ke aplikasi.

    - Registrasi
       <!-- TODO: show image design of login page here -->
        Halaman ini digunakan oleh pengguna untuk melakukan registrasi akun aplikasi jika sebelumnya belum memiliki akun. Pada halaman ini memiliki beberapa data yang harus di isi
        ```jsonc
        {
            "name": "example user",
            "adddress": "adddress of example user",
            "phone": "08xxxxxxxxxx",
            "email": "example@gmail.com",
            "password": "example_password"
        }
        ```

    - Beranda
       <!-- TODO: show image design of login page here -->
        Beranda adalah halaman yang akan dikunjungi pengguna pertama kali setelah login. Halaman ini akan menampilkan beberapa data yang terkait dengan pengguna aplikasi penjemputan sampah seperti yang terlihat pada design diatas, beberapa data yang akan ditampilkan diantaranya sebagai berikut :
       - halaman ini akan menampilkan nama pengguna yang masuk ke aplikasi dibagian paling atas
       - menampilkan jumlah point pengguna
       - jumlah total pesanan penjemputan yang sudah dilakukan pengguna <!-- TODO: added explanation of this total calculated in a period of how many days/month, for example every 1 month-->
       - jumlah total pesanan yang statusnya masih dalam proses 
       - jumlah total pesanan yang statusnya sudah selesai

    - Tukar Point
       <!-- TODO: show image design of login page here -->
    - Pickup
       <!-- TODO: show image design of login page here -->
    - Profil
       <!-- TODO: show image design of login page here -->
    - Edit Profil
       <!-- TODO: show image design of login page here -->
    - Kwitansi
       <!-- TODO: show image design of login page here -->
    - Hubungi Kami
       <!-- TODO: show image design of login page here -->

# Description
aplikasi ini 
