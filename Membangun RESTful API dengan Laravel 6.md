# Intro
## Apa itu Web Service dan REST API
1.  Apa yang dimaksud dengan web service...

    a.  A computer programming system created by Donald E. Knuth as the first implementation of what he called "literate programming"
    
    **b.  A server running on a computer device, listening for requests at a particular port over a network, serving web documents (HTML, JSON, XML, images)**
    
    c.  A software architectural style that was created to guide the design and development of the architecture for the World Wide Web.
    
    d.  Semua salah
 
2.  Dibawah ini beberapa keuntungan dari web sercive, kecuali...

    a.  Usability
    
    b.  Interoperability
    
    c.  Reusability
    
    **d.  Work Overload**
 
3.  Apa hal-hal yang perlu diperhatikan dalam membangun sebuah web services...

    a.  Latency
    
    b.  Security
    
    c.  Authentication & Authorization
    
    **d.  Semua Benar**

4.  REST merupakan kepanjangan dari...

    **a.  Representational State Transfer**
    
    b.  Representational Status Transfer
    
    c.  Recommended State Transfer
    
    d.  Representational State Transaction

5.  Apa yang dimaksud dengan REST...

    a.  A computer programming system created by Donald E. Knuth as the first implementation of what he called "literate programming".
    
    b.  A server running on a computer device, listening for requests at a particular port over a network, serving web documents (HTML, JSON, XML, images).
    
    **c.  A software architectural style that defines a set of constraints to be used for crating web services.**
    
    d.  Semua salah

6.  Dibawah ini prinsip dari sebuah REST

    a.  API defined by URI (Uniform Resource Identifier)
    
    b.  Operations: HTTP Verb (GET, POST, PUT, DELETE)
    
    c.  Stateless
    
    **d.  Semua Benar**

## Persiapan Project

7.  Pada persiapan project kita mengclone sebuah repositori dari link berikut...

    a.  https://github.com/idstck/wireshop
    
    **b.  https://github.com/idstck/laravel-restapi/**
    
    c.  https://github.com/idstck/telegram-chatbot
    
    d.  https://github.com/idstck/chatroom
 
8.  Pada materi persiapan project, perintah git dalam mengclone repositorinya yaitu...

    a.   git clones https://github.com/idstck/laravel-restapi.git restapi
    
    b.   git clone https://github.com/idstck/laravel-restapi.git restapi
    
    **c.   git klon https://github.com/idstck/laravel-restapi.git restapi**
    
    d.   git cone https://github.com/idstck/laravel-restapi.git restapi
 
## Browse API Endpoint
9.  Pada pembuatan web services laravel menyediakan file route khusus yaitu...

    a.  console.php
    
    **b.  api.php**
    
    c.  web.php
    
    d.  channels.php

10. Pada materi Browse API Endpoint, contoh code untuk menampilkan seluruh data dari tabel post, pada PostController.php adalah...
```

    **a.  public function index()
        {
            $data = Post::all();
            return response()->json($data, 200);
        }**
    
    b.  public function index()
        {
            data = Post::all();
            return response()->json($data, 200);
        }
    
    c.  public function index()
        {
            $data = Post();
            return response()->json($data, 200);
        }
    
    d.  public function index()
        {
            $data = Post::all();
            response()->json($data, 200);
        }
```

11. Software yang dapat kita gunakan untuk mengetest API Endpoint yang kita buat adalah...

    a.  Contentful
    
    **b.  Postman**
    
    c.  Mailtrap
    
    d.  Semua salah

12. Kita bisa melihat perbedaan dari penggunaan route api dan route web pada sebuah file yang bernama...

    a.  channels.php
    
    b.  console.php
    
    c.  web.php
    
    **d.  kernel.php**

## Read API Endpoint
Pada materi Read API Endpoint, contoh code untuk menampilkan salah satu data dari tabel post, pada PostController.php adalah...
```

    a.  public function show()
        {
            $data = Post::find($id);
            return response()->json($data, 200);
        }
    
    b.  public function show($id)
        {
            $data = Post::find();
            return response()->json($data, 200);
        }
    
    **c.  public function show($id)
        {
            $data = Post::find($id);
            return response()->json($data, 200);
        }**
    
    d.  public function show($id)
        {
            $data = find($id);
            return response()->json($data, 200);
        }
```

14. Berdasarkan Materi Read API Endpoint, lengkapi titik titik yang ada pada code berikut `Route::get('/post/...', 'PostController@show');`

    a.  {data}
    
    **b.  {id}**
    
    c.  {post}
    
    d.  {user}

15. Apa yang akan kita dapatkan apabila kita memasukan id data yang tidak ada dalam tabel database...

    **a.  Data kosong**
    
    b.  Aplikasi error
    
    c.  Otomatis membuat data baru
    
    d.  Semua salah

16. Apa hasil yang dikeluarkan dari menampilkan salah satu data...

    a.  Menampilkan nilai array dengan banyak data
    
    b.  Menampilkan data dari parameter yang kita masukan sampai akhir data
    
    **c.  Menampilkan satu object data saja**
    
    d.  Semua salah

