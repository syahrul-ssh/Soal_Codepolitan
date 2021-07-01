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
    
    **b.   git clone https://github.com/idstck/laravel-restapi.git restapi**
    
    c.   git klon https://github.com/idstck/laravel-restapi.git restapi
    
    d.   git cone https://github.com/idstck/laravel-restapi.git restapi
    
# Bread Api Endpoint
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

# Error Handling And Exception
## Custom Response untuk Data Tidak Ditemukan
29. Apa arti dari status code 404 yang digunakan pada response yang telah dibuat...

    a.  ok
    
    b.  created
    
    c.  accepted
    
    **d.  Not Found**

30. Berdasarkan materi Error Handling And Exception, lengkapilah titik titik pada code berikut `is_null(...)`

    **a.  $data**
    
    b.  $post
    
    c.  $user
    
    d.  semua salah

31. Berdasarkan materi Error Handling And Exception, lengkapilah titik titik pada code berikut `'...' => 'Resource not found!'`

    a.  file
    
    b.  exception
    
    **c.  message**
    
    d.  trace

32. Berdasarkan materi Error Handling And Exception, tipe data apa yang digunakan untuk response yang kita buat... 

    a.  xml
    
    b.  javascript
    
    c.  text
    
    **d.  json**

## Menambahkan Validasi beserta Responsenya
33. Berdasarkan materi Menambahkan Validasi beserta Responsenya, lengkapilah titik titik pada code berikut ini `...::make`

    a.  Validation
    
    **b.  Validator**
    
    c.  Validate
    
    d.  Valid

34. Berdasarkan materi Menambahkan Validasi beserta Responsenya, lengkapilah titik titik pada code berikut ini `'...' => ['required', 'min:5']`

    a.  body
    
    b.  user_id
    
    **c.  title**
    
    d.  id

35. Berdasarkan materi Menambahkan Validasi beserta Responsenya, lengkapilah titik titik pada code berikut ini `$validator->...`

    a.  fail()
    
    b.  failed()
    
    **c.  fails()**
    
    d.  semua salah

36. Apa arti dari status code 400 yang digunakan pada response yang telah dibuat...

    **a.  bad request**
    
    b.  created
    
    c.  accepted
    
    d.  not found

# Api Resource
## Membuat Custom Response
37. Pada laravel, kita bisa untuk tidak menampilkan/menyembunyikan sebuah atau beberapa kolom yang ada di tabel database dengan menggunakan property...

    a.  $guarded
    
    **b.  $hidden**
    
    c.  $this
    
    d.  semua salah

38. Berdasarkan materi Membuat Custom Response, kita dapat melakukan generating resources menggunakan perintah artisan...

    a.  php artisan resource Post/PostResource
    
    b.  php make Post/PostResource
    
    c.  php artisan make:resource PostResource
    
    **d.  php artisan make:resource Post/PostResource**

39. Berdasarkan materi Membuat Custom Response, lengkapilah titik titik pada code berikut ini `'stored_at' => $this->created_at->...`

    **a.  diffForHumans()**
    
    b.  diffAsCarbonInterval()
    
    c.  diff()
    
    d.  diffInMonths()

40. Berdasarkan materi Membuat Custom Response, lengkapilah titik titik pada code berikut ini `return new PostResource(...);`

    **a.  $data**
    
    b.  $this
    
    c.  $post
    
    d.  $get

41. Kita bisa membuat/mengubah property dengan property baru yang tidak ada di tabel database dengan...

    a.  $hidden
    
    **b.  $appends**
    
    c.  $this
    
    d.  semua salah

## Menggunakan Resource Collection
42. kita disarankan untuk menggunakan resource collection saat...

    **a.  Menampilkan banyak data, mengubah format, dan menambahkan metadata**
    
    b.  Menampilkan resource dalam suatu object
    
    c.  Menampilkan sebagian data
    
    d.  semua salah

43. Berdasarkan materi Menggunakan Resource Collection, lengkapilah titik titik pada code berikut ini `php artisan make:resource Post/...`

    a.  PostData
    
    b.  PostResource
    
    **c.  PostCollection**
    
    d.  PostGeneration

44. Berdasarkan materi Menggunakan Resource Collection, lengkapilah titik titik pada code berikut ini `return new ...($data);`

    a.  PostData
    
    b.  PostResource
    
    **c.  PostCollection**
    
    d.  PostGeneration

45. Berdasarkan materi Menggunakan Resource Collection, lengkapilah titik titik pada code berikut ini `...::collection($this->collection),`

    a.  PostData
    
    **b.  PostResource**
    
    c.  PostCollection
    
    d.  PostGeneration

46. Berdasarkan materi Menggunakan Resource Collection, lengkapilah titik titik pada code berikut ini `$this->...->count()`

    a.  generation
    
    b.  data
    
    c.  resource
    
    **d.  collection**

## Membuat Response Pagination
47. Salah satu dari keuntungan menggunakan resource collection pada laravel...

    a.  dapat membuat loading pemanggilan data menjadi lebih lambat
    
    **b.  dapat membuat pagination dengan mudah**
    
    c.  Dapat memudahkan dalam memberi komentar
    
    d.  semua salah

48. Berdasarkan materi Membuat Response Pagination, lengkapilah titik titik pada code berikut ini `$data = Post::...(4);`

    **a.  paginate**
    
    b.  all
    
    c.  find
    
    d.  semua salah

49. Pada saat kita menggunakan method paginate, secara otomatis laravel akan menggenerate property/data ... pada tampilan response di postman

    a.  data
    
    b.  meta
    
    **c.  links**
    
    d.  semua salah

50. Dibawah ini beberapa meta data yang terbuat saat kita membuat pagination di laravel...

    a.  last_page
    
    b.  per_page
    
    c.  current_page
    
    **d.  semua benar**

## Memuat Data Berelasi di API Resource
51. Pada awal materi Memuat Data Berelasi di API Resource, kita memanggil method user di dalam PostResource, dibawah ini peroperty yang ditampilkan setelah kita memanggil method user tersebut, kecuali...

    a.  id
    
    **b.  nama**
    
    c.  email
    
    d.  email_verified_at

52. Berdasarkan materi Memuat Data Berelasi di API Resource, perintah artisan untuk membuat User Resource adalah...

    a. php make:resource User/UserResource 
    
    b.  php artisan resource User/UserResource
    
    **c.  php artisan make:resource User/UserResource**
    
    d.  php artisan make:resource UserResource

53. Berdasarkan Memuat Data Berelasi di API Resource, lengkapilah titik titik pada code berikut `'user' => new UserResource($this->...),`

    a.  body
    
    b.  comment
    
    c.  post
    
    **d.  user**

54. Berdasarkan Memuat Data Berelasi di API Resource, lengkapilah titik titik pada code berikut `DB::listen(function ($...)`

    a.  eloquent
    
    **b.  query**
    
    c.  post
    
    d.  semua salah

55. Berdasarkan Memuat Data Berelasi di API Resource, lengkapilah titik titik pada code berikut `Post::with(['...', ])->paginate(4);`

    a.  body
    
    b.  comment
    
    c.  post
    
    **d.  user**

