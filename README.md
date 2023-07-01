# MVP of Garbage Pickup App

- ## Database Schema
    - [Schema](https://dbdiagram.io/embed/649fab0202bd1c4a5e55430f)

- ## List pages
    - Login Page

        Halaman ini ditampilkan ketika pengguna akan masuk ke aplikasi, halaman ini akan memiliki 2 opsi untuk masuk/login :
        - Login With App Account
        
            untuk login menggunakan akun yang sudah terdaftar diaplikasi, beberapa input yang harus dilakukan pengguna untuk login denga opsi ini adalah
            - `email`: `string {max: 255}`  
            - `password`: `string {min: 8}`

            example
            ```jsonc
            {
                "email": "example@gmail.com",
                "password": "xxxxxxxx", 
            }
            ```

        - Login With Google Account

	- register page
