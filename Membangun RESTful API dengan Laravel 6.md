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
13. Pada materi Read API Endpoint, contoh code untuk menampilkan salah satu data dari tabel post, pada PostController.php adalah...
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

## Add API Endpoint
17. Berdasarkan materi Add API Endpoint, contoh code untuk menambahkan satu data ke tabel post, pada PostController.php adalah...
```

    a.  public function store(Request $request)
        {
            $data = $request->all();
            $response = Post($data);
            return response()->json($response, 201);
        }
    
    b.  public function store(Request $request)
        {
            $data = $request->all();
            $response = create($data);
            return response()->json($response, 201);
        }
    
    c.  public function store()
        {
            $data = $request->all();
            $response = Post::create($data);
            return response()->json($response, 201);
        }
    
    **d.  public function store(Request $request)
        {
            $data = $request->all();
            $response = Post::create($data);
            return response()->json($response, 201);
        }**
```

18. Berdasarkan Materi Add API Endpoint, lengkapi titik titik yang ada pada code berikut `Route::post('/post', 'PostController@...');`

    **a.  store**
    
    b.  show
    
    c.  index
    
    d.  update

19. Apa arti dari status code 201 yang digunakan pada response yang telah dibuat...

    a.  ok
    
    **b.  created**
    
    c.  accepted
    
    d.  reset content

20. Pada aplikasi postman saat kita akan memasukan inputan yang akan kita masukan ke tabel database, kita bisa menggunakan tab...

    **a.  body**
    
    b.  header
    
    c.  test
    
    d.  params

## Edit API Endpoint
21. Berdasarkan materi Edit API Endpoint, contoh code untuk mengedit satu data ke tabel post, pada PostController.php adalah...
```

    a.  public function (Request $request, Post $post)
    
        {
        
            $post->update($request->all());
            
            return response()->json($post, 200);
            
        }
    
    **b.  public function update(Request $request, Post $post)
    
        {
        
            $post->update($request->all());
            
            return response()->json($post, 200);
            
        }**
    
    c.  public function update(Request $request)
    
        {
        
            $post->update($request->all());
            
            return response()->json($post, 200);
            
        }
    
    d.  public update(Request $request, Post $post)
    
        {
        
            $post->update($request->all());
            
            return response()->json($post, 200);
            
        }
```

22. Berdasarkan Materi Edit API Endpoint, lengkapi titik titik yang ada pada code berikut `Route::...('/post/{post}', 'PostController@update');`

    a.  get
    
    b.  post
    
    **c.  put**
    
    d.  update

23. Apa arti dari status code 200 yang digunakan pada response yang telah dibuat...

    **a.  ok**
    
    b.  created
    
    c.  accepted
    
    d.  reset content

24. Berdasarkan materi Edit API Endpoint, kita menambahkan sebuah parameter `Post $post` didalam function update yang kita buat, parameter tersebut adalah implementasi dari...

    a.  Migrations
    
    b.  API Resources
    
    c.  Eloquent
    
    **d.  Route Model Binding**

## Delete API Endpoint
25. Berdasarkan materi Delete API Endpoint, contoh code untuk Menghapus satu data ke tabel post, pada PostController.php adalah...
```

    a.  public function(Post $post)
        {
            $post->delete();
            return response()->json(null, 200);
        }
    
    b.  public destroy(Post $post)
        {
            $post->delete();
            return response()->json(null, 200);
        }
    
    **c.  public function destroy(Post $post)
        {
            $post->delete();
            return response()->json(null, 200);
        }**
    
    d.  public function destroy($post)
        {
            $post->delete();
            return response()->json(null, 200);
        }
```

26. Berdasarkan Materi Delete API Endpoint, lengkapi titik titik yang ada pada code berikut `Route::delete('/post/{post}', 'PostController@...');`

    a.  get
    
    **b.  destroy**
    
    c.  put
    
    d.  update

27. Kita bisa menghapus sebuah data pada object eloquent bisa menggunakan sebuah method berikut...

    **a.  delete()**
    
    b.  post()
    
    c.  get()
    
    d.  update()

28. Apa status code Http yang akan kita terima apabila kita menghapus sebuah data yang memang tidak ada...

    a.  201
    
    b.  200
    
    **c.  404**
    
    d.  403
