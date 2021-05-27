# Persiapan Awal
## Menginstall Laravel
1.	Kita dapat mengakses website Laravel dengan memasuki link sebagai berikut…

    **a.	Laravel.com**
    
    b.	Laracast.com
    
    c.	Laragon.com
    
    d.	Google.com 
    
2. Butuh minimal versi PHP berapa untuk dapat menginstall Laravel 6…

    a.	7.2.3
    
    b.	7.1.4
    
    **c.	7.1.3**
    
    d.	7.1.2
    
3. Bagaimana cara mengintall laravel menggunakan composer…

    a.	composer project-create --prefer-dist laravel/laravel blog
    
    **b.	composer create-project --prefer-dist laravel/laravel blog**
    
    c.	composer laravel/laravel create-project --prefer-dist blog
    
    d.	composer --prefer-dist create-project laravel/laravel blog
    
## Struktur Project Laravel
4.	Yang berfungsi sebagai jembatan antara model dan view adalah…

    a.	Middleware
    
    **b.	Controller**
    
    c.	Routes
    
    d.	Migration 
    
5. File/folder tempat kita untuk membuat tabel untuk database pada laravel…

    a.	Middleware
    
    b.	Controller
    
    c.	Routes
    
    **d.	Migration** 
    
6. Sebuah entry point yang kita gunakan untuk mendaftarkan URL yang ada di website kita…

    a.	Middleware
    
    b.	Controller
    
    **c.	Routes**
    
    d.	Migration 
    
## Perintah Artisan
7.	Didirectory mana kita dapat mengeksekusi perintah artisan...

    a.	Di Dalam Folder App
    
    b.	Di Dalam Folder Bootstrap
    
    c.	Di Dalam Folser Resource
    
    **d.	 Di Root Folder Project**
    
8. Perintah artisan untuk memasukan project kita kedalam mode maintenance...

    a.	php artisan migrate
    
    **b.	php artisan down**
    
    c.	php artisan serve
    
    d.	php artisan tinker
    
9. Perintah artisan untuk menjalankan local development server dalam laravel...

    a.	php artisan migrate
    
    b.	php artisan down
    
    **c.	php artisan serve**
    
    d.	php artisan tinker
    
## Mengatur App Key
10. Apa fungsi dari perintah artisan app key:generate...

    a.	Membuat migration pada aplikasi
    
    b.	Membuat controller pada aplikasi
    
    **c.	Membuat key pada aplikasi**
    
    d.	 Membuat route pada applikasi
    
11. Apa fungsi dari app key yang terdapat pada laravel...

    a.	Membuat aplikasi menjadi lebih keren
    
    **b.	Memberikan keamanan bagi aplikasi**
    
    c.	Membuat aplikasi mudah diretas
    
    d.	Membuat aplikasi menjadi lebih berat
    
12. Apa yang akan terjadi apabila aplikasi laravel kita tidak memiliki app key

    **a.	Aplikasi tidak dapat diakses atau terdapat error**
    
    b.	Aplikasi berjalan dengan semestinya
    
    c.	Aplikasi menjadi sangat ringan
    
    d.	Semua Salah
    
## Namespace Aplikasi
13. Perintah Artisan untuk mengubah namespace adalah...

    a.	php artisan name:app BelajarLaravel
    
    b.	php artisan names:apps BelajarLaravel
    
    c.	php artisan apps:names BelajarLaravel
    
    **d.	 php artisan app:name BelajarLaravel**
    
14. Pada saat menjalankan perintah artisan untuk mengubah namespace, file mana sajakah yang akan terganti namespacenya

    **a.	Seluruh namespace yang ada di aplikasi berubah**
    
    b.	Sebagian namespace yang ada di aplikasi berubah
    
    c.	Hanya salah satu file yang sedang dibuka akan berubah
    
    d.	Semua Salah
    
## Namespace Aplikasi  
15. folder yang digunakan untuk melakukan konfigurasi pada laravel

    **a.	config**
    
    b.	controller
    
    c.	route
    
    d.	public
16. Alternatif untuk melakukan konfigurasi aplikasi laravel selain di dalam foldernya kita bisa menggunakan... 

    a.	.editorconfig
    
    b.	.gitigrone
    
    **c.	.env**
    
    d.	 artisan
    
17. Apakah mungkin untuk membuat file konfigurasi baru di dalam folder config

    a.	tidak bisa
    
    **b.	ya, bisa**
    
18. Bagaimana kita dapat mengakses konfigurasi melalui route

    **a.	return config('majalah.pagination');**
    
    b.	return post('majalah.pagination');
    
    c.	return get('majalah.pagination');
    
    d.	Semua Salah
    
# Routing Di Laravel
## Mengenal Routing
19.	File routing yang digunakan untuk membuat sebuah halaman website bernama...
    **a.	web.php**
    
    b.	console.php
    
    c.	channel.php
    
    d.	api.php
    
20. Default routing yang disediakan laravel 6 pada web.php adalah...

```
    a.	Route::post('/', function (){
            return view('welcome');
         });
    
    b.	Route::get('/', function (){
            return ('welcome');
         });
    
    **c.	Route::get('/', function (){
            return view('welcome');
         });**
    
    d.	Route::put('/', function (){
            return view('welcome');
         });
```
    
21. Method untuk mengambil/menampilkan data pada routing adalah dengan...

    a.	post
    
    **b.	get**
    
    c.	put
    
    d.	delete
## Parameter pada Route
22. Fungsi dari route parameter adalah...

    a.	Untuk menampilkan web dengan cepat
    
    b.	Untuk membuat data lebih tertatarapih di database
    
    **c.	Untuk menampilkan data berdasarkan parameter tertentu seperti id atau username**
    
    d.	Untuk menampilkan langsung semua data yang ada pada database 
    
23. Contoh dari pembuatan routing parameter pada laravel...
```

    a.	Route::get('/', function (){
            return view('welcome');
         });
    
    **b.	Route::get('/user/{id}', function ($id){
            return 'user ' . $id;
         });**
    
    c.	Route::get('/user/{id}', function (){
            return 'user ' . $id;
         });
    
    d.	Route::post('/user/id', function ($id){
            return 'user ' . $id;
         });
```
    
24. Contoh dari pembuatan routing parameter yang mana parameter tersebut menjadi optional atau bisa tidak diisi pada laravel...
```

    **a.	Route::get('/user/{id?}', function ($id = null){
            return 'user ' . $id;
         });**
    
    b.	Route::get('/user/{id}', function ($id = null){
            return 'user ' . $id;
         });
    
    c.	Route::get('/user/{id?}', function ($id){
            return 'user ' . $id;
         });
    
    d.	Route::get('/user/{id}', function ($id){
            return 'user ' . $id;
         });
```
         
## Route Group
25. Contoh dari penulisan route group pada laravel...
```

    a.	Route::get('/user/{id}', function ($id){
            return 'user ' . $id;
         });
    
    **b.	Route::prefix('user')->group(function(){
               Route::get('/change-password', function (){
                  return 'change-password';
               });
         });**
    
    c.	Route::prefix('user'){
               Route::get('/change-password', function (){
                  return 'change-password';
               });
         });
    
    d.	Route::get('user')->group(function(){
               Route::get('/change-password', function (){
                  return 'change-password';
               });
         });
```
    
26. Fungsi dari route group pada laravel adalah

    **a.	Untuk mengumpulkan route yang memiliki prefix yang sama**
    
    b.	Untuk memisahkan route yang memiliki prefix yang sama
    
    c.	Untuk menghapus route yang memiliki prefix yang sama
    
    d.	Untuk mengedit route yang memiliki prefix yang sama
    
27. Apakah bisa kita membuat route group di dalam route group...

    a.	Tidak bisa
    
    **b.	Ya, bisa**
    
## Route Alias Name
28. Apa fungsi dari menggunakan alias name pada routing laravel...

    a.	memperumit codingan
    
    b.	mempersulit dalam memanggil url pada website
    
    **c.	mempermudah atau mempersingkat url yang bisa kita panggil nantinya**
    
    d.	semua salah
    
29. Contoh dari pembuatan alias name pada routing laravel...
```

    a.	Route::get('homapage/landing-page', function (){
            return 'landing';
         })->nama('homepage');
    
    **b.	Route::get('homapage/landing-page', function (){
            return 'landing';
         })->name('homepage');**
    
    c.	Route::get('homapage/landing-page', function (){
            return 'landing';
         })->alias('homepage');
    
    d.	Route::get('homapage/landing-page', function (){
            return 'landing';
         })->names('homepage');
```
    
30. Contoh dari code pemanggilan alias name pada routing laravel...
```

    **a.	Route::get('redirect', function (){
            return redirect()->route('homepage');
         });**
    
    b.	Route::get('redirect', function (){
            return redirect()->name('homepage');
         });
    
    c.	Route::get('redirect', function (){
            return redirect()->middleware('homepage');
         });
    
    d.	Route::get('redirect', function (){
            return redirect()->alias('homepage');
         });
```

## Route Resource dan API Resource
31. Apa fungsi dari route resource pada laravel...

    a.	memperumit codingan
    
    **b.	Untuk mempermudah dalam pembuatan routing untuk CRUD**
    
    c.	Untuk mempersulit dalam pembuatan routing untuk CRUD
    
    d.	semua salah
    
32. Contoh dari pembuatan route resource pada laravel...
```

    **a.	Route::resource('article', 'ArticleController');**
    
    b.	Route::get('article', 'ArticleController');
    
    c.	Route::post('article', 'ArticleController');
    
    d.	Route::delete('article', 'ArticleController');
```
    
33. Contoh dari perintah artisan dalam membuat controller untuk sebuah route resource yang telah kita buat...

    a.	php artisan make:controller ArticleController --route
    
    b.	php artisan controller:make ArticleController --resource
    
    **c.	php artisan make:controller ArticleController --resource**
    
    d.	php artisan make:controller ArticleController
    
34. Contoh dari pembuatan route resource pada laravel...
```

    a.	Route::apiRoute('article', 'ArticleController');
    
    **b.	Route::apiResource('article', 'ArticleController');**
    
    c.	Route::resource('article', 'ArticleController');
    
    d.	Route::api('article', 'ArticleController');
```
    
## Route View dan Redirect
35. Apa fungsi dari route view...

    a.	Untuk mengalihkan sebuah halaman ke halaman yang kita inginkan
    
    **b.	Untuk menampilkan sebuah view dari file yang ingin kita tampilkan**
    
    c.	Untuk mempermudah dalam pembuatan route lain
    
    d.	Untuk Menampilkan route list
    
36. Apa fungsi dari route redirect...

    **a.	Untuk mengalihkan atau meredirect sebuah halaman ke halaman yang kita inginkan**
    
    b.	Untuk menampilkan sebuah view dari file yang ingin kita tampilkan
    
    c.	Untuk mempermudah dalam pembuatan route lain
    
    d.	Untuk Menampilkan route list
