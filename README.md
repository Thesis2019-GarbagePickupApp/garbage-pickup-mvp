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

       Halaman ini merupakan tempat di mana pengguna dapat menukarkan point yang telah mereka kumpulkan dengan berbagai voucher terkait aplikasi penjemputan sampah. Di halaman ini, pengguna dapat memilih dari berbagai pilihan voucher yang tersedia, seperti diskon 10% atau voucher sejenisnya. Pengguna dapat menggunakan point mereka sebagai mata uang untuk mendapatkan manfaat tambahan dalam penggunaan aplikasi, membrikan penghargaan atas kontribusi mereka dalam menjaga kebersihan lingkungan. Diharapkan halaman ini dapat memberikan pengalaman yang mudah dan menyenangkan bagi pengguna untuk menukarkan poin mereka dengan berbagai voucher menarik.
       Beberapa data yang akan ditampilkan di halaman ini adalah sebagai berikut :
       - total poin pengguna yang dapat ditukarkan dengan voucher yang tersedia
       - data voucher seperti deskripsi, point yang diperlukan untuk ditukarkan, jenis voucher, dan jumlah potongan harga

    - Pickup
       <!-- TODO: show image design of login page here -->

       Halaman Pickup dalam aplikasi penjemputan sampah dapat digunakan oleh pengguna untuk melakukan permintaan penjemputan sampah. Di halaman ini, pengguna akan diminta untuk memasukan beberapa data penting untuk keperluan penjemputan sampah seperti lokasi penjemputan, jenis sampah, dan berat sampah yang akan di angkut dalam satuan KG (Kilo Gram).
       - lokasi/tempat penjemputan

         Pengguna akan memberikan informasi mengenai tempat penjemputan, baik itu alamat rumah atau koordinat lokasi yang spesifik. Hal ini memungkinkan pengemudi sampah untuk mengetahui dengan jelas dimana pengguna membutuhkan penjemputan sampah.

       - jenis sampah

            Pengguna akan memilih jenis sampah yang akan diangkut. Seperti organik, anorganik, plastik, kertas atau karton, logam, kaca, elektronik atau jenis sampah lainnya. Dengan menentukan jenis sampah, pengemudi sampah dapat melakukan pemisahan sampah dengan efisien dan pengatur penjemputan sesuai dengan jenis sampah yang diminta.

       - berat sampah

            Pengguna akan memasukan berat sampah yang akan diangkut. Hal ini penting untuk membantu pengemudi sampah menentukan ukuran dan kapasitas kendaraan yang dibutuhkan, serta mengatur jadwal penjemputan dengan lebih baik.

    - Profil
       <!-- TODO: show image design of login page here -->

       Halaman "Profil" dalam aplikasi penjemputan sampah berguna untuk menampilkan informasi pengguna seperti  nama, alamat, nomor hp, email, dan password. Halaman ini dirancang untuk memberikan gambaran tentang identitas pengguna dan memberikan akses untuk mengelola data pribadi mereka.
       Selain itu, terdapat tombol "Edit Akun" yang memungkinkan pengguna untuk mengubah data mereka. Dengan mengeklik tombol ini pengguna akan diarahkan ke halaman pengeditan dimana mereka dapat memperbarui informasi profil seperti alamat, nomor telepon, atau alamat email. Selain itu, pengguna dapat merubah kata sandi atau password mereka jika diperlukan.

    - Edit Profil
       <!-- TODO: show image design of login page here -->

       Halaman "Edit Profil" merupakan halaman lanjutan dari halaman "Profil" ketika tombol "Edit Akun" diklik. Halaman ini memungkinkan pengguna untuk mengedit informasi pribadi mereka dengan mudah. 

       Pada halaman "Edit Profil", pengguna akan melihat formulir atau bidang yang dapat diubah yang mencakup data seperti nama, alamat, nomor telepon, alamat email, dan kata sandi. Pengguna dapatmengisi bidang-bidang tersebut dengan informasi baru yang ingin mereka perbarui.

       Setelah pengguna mengubah data yang ingin mereka update, mereka dapat menyimpan perubahan dengan mengeklik tombol "Simpan" yang ada dihalaman. Tombol ini akan mengirimkan perubahan yang dilakukan ke sistem dan memperbarui informasi profil pengguna. 

       Halaman "Edit Profil" memberikan pengguna kontrol penuh untuk mengubah dan memperbarui informasi pribadi mereka sesuai kebutuhan. Ini memungkinkan pengguna untuk memperbarui data profil mereka dengan mudah dan memberikan fleksibilitas dalam mengelola informasi yang terkait dengan akun mereka

    - Kwitansi
       <!-- TODO: show image design of login page here -->

    - Hubungi Kami
       <!-- TODO: show image design of login page here -->

# Description
aplikasi ini 
