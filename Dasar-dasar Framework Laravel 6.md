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

# Menggunakan Controller dan View
## Mengenal Controller
37. Perintah artisan untuk membuat sebuah controller adalah...

    a.	php artisan controller:make HomeController
    
    **b.	php artisan make:controller HomeController**
    
    c.	php artisan controller HomeController
    
    d.	php artisan makes:controller HomeController

38. Apa fungsi dari sebuah controller pada laravel...

    a.	Sebagai penghubung antara route dan resource
    
    b.	Sebagai penghubung antara config dan database
    
    **c.	Sebagai penghubung antara model dan view**
    
    d.	semua salah

39. Contoh pembuatan route untuk controller pada laravel... 

    **a.	Route::get('user', 'HomeController@index')->name('user');**
    
    b.	Route::get('user', 'HomeController')->name('user');
    
    c.	Routes::get('user', 'HomeController@index')->name('user');
    
    d.	Route::get('user', '@index')->name('user');
    
## Controller Object Request
40. Class apa yang akan selalu di import saat membuat controller menggunakan artisan...

    a.	use Http\Illuminate\Request;
    
    b.	use Request\Http\Illuminate;
    
    c.	use Http\Request\Illuminate;
    
    **d.	use Illuminate\Http\Request;**

41. Fungsi dari class request pada controller laravel adalah...

    a.	Menggantikan fungsi controller
    
    **b.	Menggantikan fungsi global GET dan POST**
    
    c.	Membuat web menjadi cepat
    
    d.	Semua salah

42. Salah satu contoh code dalam mengambil parameter dengan request...

    a.	echo $request->post('nama');
    
    b.	echos $request->get('nama');
    
    **c.	echo $request->get('nama');**
    
    d.	Semua salah
    
## Controller untuk Submit Form
43. Contoh pembuatan route post untuk controller pada laravel... 

    a.	Routes::post('user', 'HomeController@index')->name('user');
    
    b.	Route::post('user', 'HomeController')->name('user');
    
    **c.	Route::post('user', 'HomeController@index')->name('user');**
    
    d.	Route::post('user', '@index')->name('user');	

44. Error apa yang akan kita temui saat kita memasukan isian form dan kita belum melakukan exception pada middleware...

    a.	404|Not Found
    
    b.	410|Gone
    
    **c.	419|Page Expired**
    
    d.	408|Request Timeout

45. Pada saat melakukan exception di folder middleware untuk form kita, di file manakah kita melakukan exception...

    a.	Authenticate.php
    
    **b.	VerifyCsrfToken.php**
    
    c.	EncryptCookies.php
    
    d.	TrimStrings.php

## Menggunakan View
46. Contoh code untuk menampilkan sebuah view dari controller pada laravel...

    a.	return user;
    
    b.	return (user.index);
    
    **c.	return view('user.index');**
    
    d.	return ('user.index');

47. Contoh code untuk menampilkan sebuah view dari controller dengan mempassing data pada laravel...

    a.	return user;
    
    b.	return (user.index)->with('username', $username);;
    
    c.	return view('user.index');
    
    **d.	return view('user.index')->with('username', $username);**

48. Contoh code untuk menampilkan sebuah view dari controller dengan menggunakan array data pada laravel...
```

    a.	return (user, [
            'username' => $username,
            'fullname' => 'Amirul Ihsan'
         ]);
    
    **b.	return view('user.index', [
            'username' => $username,
            'fullname' => 'Amirul Ihsan'
         ]);**
    
    c.	return ('user.index', [
            'username' => $username,
            'fullname' => 'Amirul Ihsan'
         ]);
    
    d.	return (user.index, [
            'username' => $username,
            'fullname' => 'Amirul Ihsan'
         ]);
```

## Kustomisasi Halaman Error
49. Error apa yang akan kita temui saat kita memasukan url yang belum terdaftar pada route milik kita...

    **a.	404|Not Found**
    
    b.	410|Gone
    
    c.	419|Page Expired
    
    d.	408|Request Timeout	

50. kita bisa mengkostumisasi halaman error dengan...

    a.	Membuatnya langsung dari route
    
    b.	Membuatnya dari controller
    
    **c.	Membuat sebuah folder di view dengan nama errors dan membuat file sesuai code errornya**
    
    d.	Semua salah

## Kustomisasi Halaman Error
51. Apa singkatan dari csrf...

    a.	Cross Site Scripting
    
    **b.	Cross-site Request Forgery**
    
    c.	Structured Query Language
    
    d.	Hyper Text Transfer Protocol

52. Serangan csrf adalah..

    a.	Serangan terhadap server website
    
    b.	Serangan yang menggunakan malware ke website
    
    c.	Serangan yang membuat hacker dapat mengetahui komunikasi antara website kita dengan server
    
    **d.	Serangan dari website lain kepada website milik kita dengan menggunakan submit form**

53. Ada berapa cara dalam menuliskan csrf_token pada video materi tentang perlindungan csrf... 

    a.	1
    
    b.	2
    
    **c.	3**
    
    d.	4	

54. Manakah salah satu contoh code dalam membuat csrf_token...

    a.	return view('user.index');
    
    **b.	@csrf**
    
    c.	Route::post('user', 'HomeController@index')->name('user');
    
    d.	echo $request->get('nama');

# Dasar-Dasar Vallidasi Form
## Mengenal Validasi Form
55.	Contoh code pada laravel untuk membuat validasi form...
```

    **a.	$this->validate($request, [
            'email' => 'required'
         ]);**
    
    b.	$this->validation($request, [
            'email' => 'required'
         ]);
    
    c.	$this->validate([
            'email' => 'required'
         ]);
    
    d.	$this->validate(request, [
            'email' => 'required'
         ]);
```

    
56. Pada video materi Mengenal Validasi Form apa yang terjadi pada form yang tidak di isi dan tidak ada validasi didalamnya...

    a.	akan kembali menampilkan form
    
    b.	membuat website menjadi error
    
    **c.	akan menampilkan data null**
    
    d.	semua salah
    
57. Pada video materi Mengenal Validasi Form apa yang terjadi pada form yang tidak di isi dan kita telah mensetting validasi di project kita ...

    **a.	akan kembali menampilkan form**
    
    b.	membuat website menjadi error
    
    c.	akan menampilkan data null
    
    d.	semua salah

## Kustomisasi Pesan Error pada Validasi
58.	Contoh code pada laravel untuk membuat kustomisasi pesan error pada validasi form...
```

    a.	$this->validation($request, [
            'email' => 'required|email'
         ], [
            'required => 'Harus Diisi'
            'email' => 'Kami membutuhkan email yang valid'
         ]);
    
    b.	$this->validate([
            'email' => 'required|email'
         ], [
            'required => 'Harus Diisi'
            'email' => 'Kami membutuhkan email yang valid'
         ]);
    
    c.	$this->validate(request, [
            'email' => 'required|email'
         ], [
            'required => 'Harus Diisi'
            'email' => 'Kami membutuhkan email yang valid'
         ]);
    
    **d.	$this->validate($request, [
            'email' => 'required|email'
         ], [
            'required => 'Harus Diisi'
            'email' => 'Kami membutuhkan email yang valid'
         ]);**
```

    
59. Kita bisa mengcustom pesan error agar bisa dinamis mengikuti dari nama atributnya dengan cara menambahkan...

    a.	:validate pesan error
    
    **b.	:attribute pesan error**
    
    c.	:accept pesan error
    
    d.	semua salah
    
60. Selain kita bisa mengkustomisasi pesan error form validation langsung dari controller, kita juga bisa mengkustomisasi pesan error form validation dari...

    **a.	validation.php**
    
    b.	passwords.php
    
    c.	pagination.php
    
    d.	auth.php
    
## Validasi Form dengan Gaya Bootstrap
61.	contoh implementasi penulisan class is-invalid pada validasi menggunakan bootstrap di laravel...
```

    **a.	{{ $errors->has('email') ? 'is-invalid' : '' }}**
    
    b.	{{ errors->has('email') ? 'is-invalid' : '' }}
    
    c.	{{ $error->has('email') ? 'is-invalid' : '' }}
    
    d.	{{ $errors->have('email') ? 'is-invalid' : '' }}
```

    
62. Pada materi Validasi Form dengan Gaya Bootstrap, kita menggunakan bootstrap versi berapa...

    a.	v4.3.3
    
    b.	v3.4.1
    
    **c.	v4.3.1**
    
    d.	v3.4.3
    
63. Pada materi Validasi Form dengan Gaya Bootstrap, kita mengcopy sebuah code dari bootstrap, code tersebut berupa script dari...

    **a.	CSS**
    
    b.	JS
    
    c.	Bundle
    
    d.	Modules

## Mengambil Nilai Request Sebelumnya (Old Request)
64. pada materi Mengambil Nilai Request Sebelumnya (Old Request), kita dapat menggunakan helper dari laravel untuk mengambil inputan sebelumnya, helper tersebut adalah...

    a.	data_get()
    
    b.	abort_if()
    
    **c.	old()**
    
    d.	str_plural()

    
65. contoh penulisan helper old() pada tag form adalah...

    a.	class="old('email')"
    
    **b.	value"{ old('email') }"**
    
    c.	type="old('email')"
    
    d.	placeholder="old('email')"

66. pada materi Mengambil Nilai Request Sebelumnya (Old Request), Apa yang terjadi saat kita menginputkan email yang tidak valid, dan kita sudah menggunakan helper old() pada formnya...

    a.	inputan akan hilang
    
    b.	inputan akan masuk langsung ke database
    
    **c.	inputan akan tetap ada seperti sebelum menekan subcribe**
    
    d.	semua salah
    
## Validasi dengan Class Form Request
67. contoh perintah artisan untuk membuat sebuah class form request...

    a.	php artisan request:make SubscriptionFormRequest
    
    **b.	php artisan make:request SubscriptionFormRequest**
    
    c.	php artisan request SubscriptionFormRequest
    
    d.	php make:request artisan SubscriptionFormRequest
    
68. File class yang telah dibuat menggunakan perintah artisan untuk membuat class form request terdapat didirectory...

    a.	app/Http/Middleware
    
    b.	app/Http/Controllers
    
    **c.	app/Http/Requests**
    
    d.	app/Http

69. pada materi Validasi dengan Class Form Request, setelah kita melakukan konfigurasi di file class form requestnya apa yang harus kita lakukan...

    **a.	menginject file class form requestnya ke dalam method yang akan kita gunakan**
    
    b.	Membiarkannya begitu saja
    
    c.	Membuat class baru dengan nama yang sama
    
    d.	Semua salah

## Response dengan Redirect
70. Apa fungsi dari redirect adalah...

    a.	kita akan tetap pada halaman yang sama
    
    **b.	mengalihkan kita ke halaman lain**
    
    c.	membantu dalam validasi form
    
    d.	semua salah
    
71. pada laravel ada sebuah method atau helper yang membantu kita melakukan redirect, method tersebut adalah...

    a.	old()
    
    **b.	redirect()**
    
    c.	route()
    
    d.	base_path()

72. pada materi Response dengan Redirect, ada beberapa cara penulisan untuk redirect, dari beberapa penulisan tersebut cara mana yang di sarankan oleh pematerinya...

    a.	return redirect('/lain');
    
    b.	return redirect()->to('/lain');
    
    **c.	return redirect()->route('other');**
    
    d.	semua salah

## Response dengan JSON
73. response menggunakan JSON biasanya digunakan untuk...

    **a.	Pembuatan dalam API yang nantinya akan dikonsumsi oleh frontend atau mobile developer**
    
    b.	mengalihkan kita ke halaman lain
    
    c.	membantu dalam validasi form
    
    d.	semua salah
    
74. pada laravel ada sebuah method atau helper yang membantu kita melakukan response dengan JSON, method tersebut adalah...

    a.	old()
    
    b.	redirect()
    
    **c.	response()->json()**
    
    d.	base_path()

## Konfigurasi Email
75. Kita bisa mengkonfigurasi untuk berkirim email di laravel pada file...

    a.	.gitignore
    
    **b.	.env**
    
    c.	artisan
    
    d.	.editorconfig
    
76. pada materi Konfigurasi Email, saat pengembangan aplikasi secara local, kita bisa mencoba untuk mengirim email menggunakan...

    a.	MailSpring
    
    b.	Apple Mail
    
    c.	Windows Mail
    
    **d.	Mailtrap**

77. Apa fungsi dari mailtrap...

    **a.	testing dalam berkirim email saat mengembangkan sebuah aplikasi, email tersebut akan ditampung di mailtrap, agar email tersebut tidak terkirim ke email sungguhan**
    
    b.	testing dalam berkirim email saat mengembangkan sebuah aplikasi, email tersebut tidak akan ditampung di mailtrap, dan email tersebut akan terkirim ke email sungguhan
    
    c.	testing dalam berkirim email saat mengembangkan sebuah aplikasi, email tersebut akan ditampung di mailtrap, dan email tersebut juga akan terkirim ke email sungguhan
    
    d.	semua salah
    
78. Driver Mail yang di support oleh laravel adalah...

    a.	smtp
    
    b.	mailgun
    
    c.	maildrill
    
    d.	semua benar

## Dasar-dasar dalam Mengirim Email
75. Perintah artisan untuk membuat class mailable pada laravel adalah...

    a.	php artisan mail:make UserVerificationMail
    
    b.	php artisan mail UserVerificationMail
    
    **c.	php artisan make:mail UserVerificationMail**
    
    d.	php make:mail artisan UserVerificationMail
    
76. pada saat kita sudah melakukan perintah artisan untuk membuat class mailable, file tersebut akan tersimpan di...

    a.	app/Http
    
    **b.	app/Mail**
    
    c.	app/Exceptions
    
    d.	app/Console

77. Contoh code yang terdapat di Controller untuk berkirim email adalah...

    a.	Mails::to('ihsan@belajarlaravel.test')->send(new UserVerificationMail());
    
    b.	Mail::to(ihsan@belajarlaravel.test)->send(new UserVerificationMail());
    
    **c.	Mail::to('ihsan@belajarlaravel.test')->send(new UserVerificationMail());**
    
    d.	semua salah
    
## Email dengan Format Markdown
78. Perintah artisan untuk membuat class mailable beserta dengan markdownnya pada laravel adalah...

    a.	php artisan mail:make UserVerificationMail --markdown='emails.activation'
    
    b.	php artisan mail UserVerificationMail --markdown='emails.activation'
    
    **c.	php artisan make:mail UserVerificationMail --markdown='emails.activation'**
    
    d.	php make:mail artisan UserVerificationMail --markdown='emails.activation'
    
79. Setelah kita membuat class mailable dengan markdown menggunakan perintah artisan, apa isi dari method build yang terdapat di class mailable dengan markdown yang telah dibuat kita buat...

    a.	return markdown('emails.activation');
    
    **b.	return $this->markdown('emails.activation');**
    
    c.	return $this->markdown(emails.activation);
    
    d.	return $this->('emails.activation');

80. Setelah kita membuat class mailable dengan markdown menggunakan perintah artisan, pada viewnya kita diberikan default code seperti apa...
```

    a.	@component('message')
    
         # Introduction
         
         
         The body of your message.
         
         
         @component('button', ['url' => ''])
         
         Button Text
         
         @endcomponent
         

         Thanks,<br>
         
         {{ config('app.name') }}
         
         @endcomponent
    
    b.	@component('mail::message')
         
         The body of your message.
         
         
         @component('mail::button')
         
         Button Text
         
         @endcomponent
         

         Thanks,<br>
         
         {{ config('app.name') }}
         
         @endcomponent
    
    **c.	@component('mail::message')
    
         # Introduction
         
         
         The body of your message.
         
         
         @component('mail::button', ['url' => ''])
         
         Button Text
         
         @endcomponent
         

         Thanks,<br>
         
         {{ config('app.name') }}
         
         @endcomponent**
    
    d.	Semua salah
    
```

## Render Email di View
81. Kita bisa melakukan pengecekan email yang dikirim oleh kita dengan merendernya didalam view dengan menambahkan code di controller sebagai berikut...

    a.	return UserActivationMail();
    
    **b.	return new UserActivationMail();**
    
    c.	return new UserActivationMail;
    
    d.	semua salah
    
82. apa keunggulan kita langsung merender tampilan email didalam view...

    a.	menghamburkan waktu pembuatan tampilan untuk email
    
    **b.	mengefisiensikan waktu dalam pembuatan tampilan untuk email, agar kita tidak selalu melihatnya di mailtrap**
    
    c.	mengefisiensikan waktu dalam pembuatan tampilan website
    
    d.	semua salah

# Menggunakan Migration
## Konsep Migration
83. Apa fungsi dari migration pada laravel...

    a.	untuk menggantikan fungsi dari database
    
    b.	untuk mempersulit dalam kolaborasi pembuatan tabel pada database
    
    **c.	untuk memudahkan dalam kolaborasi pembuatan tabel pada database**
    
    d.	semua salah
    
84. Berada di directory mana migration ini berada...

    a.	app/Http/Controllers
    
    **b.	database/migrations**
    
    c.	database/factories
    
    d.	database/seeds
    
85. perintah artisan untuk membuat sebuah file migration pada laravel adalah...

    a.	php make:migration create_users_table
    
    b.	php artisan migration:make create_users_table
    
    c.	php artisan migration create_users_table
    
    **d.	php artisan make:migration create_users_table**
    
86. perintah artisan untuk menjalankan file migration yang telah kita buat adalah...

    a.	php artisan optimize
    
    **b.	php artisan migrate**
    
    c.	php artisan serve
    
    d.	php artisan up

## Memodifikasi Kolom
87. pada materi Memodifikasi Kolom, pemateri menyampaikan bahwa cara terbaik dalam memodifikasi tabel dalam database menggunakan migration yaitu dengan...

    a.	mengedit file migration yang sudah ada
    
    **b.	membuat file migration baru**
    
    c.	menghapus file migration yang lama, lalu membuat lagi yang baru
    
    d.	semua salah
    
88. pada materi Memodifikasi Kolom, saat kita ingin merubah suatu kolom pada file migration, kita harus menambahkan method...

    a.	edit();
    
    **b.	change();**
    
    c.	store();
    
    d.	update();
    
89. pada materi Memodifikasi Kolom, saat kita melakukan php artisan migrate itu terjadi sebuah error, error tersebut mengharuskan kita untuk menginstall dependency sebagai berikut...

    a.	spatie/laravel-menu
    
    b.	lubusin/laravel-decomposer
    
    **c.	doctrine/dbal**
    
    d.	semua salah

# Managemen Database dengan Eloquent
## Membuat Model dan Data
90. pada migration tabel posts kita bisa lihat ada kolom yang bernama created_at dan updated_at, kedua kolom tersebut terbuat dari method...

    a.	string();
    
    **b.	timestamps();**
    
    c.	date();
    
    d.	time();
    
91. perintah artisan untuk membuat sebuah model pada laravel yaitu...

    a.	php artisan model Post
    
    b.	php make:model Post
    
    **c.	php artisan make:model Post**
    
    d.	php artisan make Post
    
92. apa fungsi dari eloquent pada laravel...

    **a.	berfungsi untuk berinteraksi dengan database**
    
    b.	berfungsi untuk berinteraksi dengan controller
    
    c.	berfungsi untuk berinteraksi dengan route
    
    d.	semua salah

93. pada model kita harus mendefinisikan kolom yang kita buat agar dapat diisi dengan data, didalam sebuah property...

    a.	$table
    
    **b.	$fillable**
    
    c.	$primary_key
    
    d.	semua salah
    
## Mengambil Data dari Database
94. dalam mengambil data dari database menggunakan eloquent, kita bisa menggunakan method...

    a.	update()
    
    b.	post()
    
    **c.	get()**
    
    d.	take()
    
95. kita bisa membatasi data yang akan kita tampilkan dengan menggunakan method...

    a.	update()
    
    b.	post()
    
    c.	get()
    
    **d.	take()**

## Membuat, Mengubah dan Menghapus Data di Database
96. contoh code dalam mengimplementasikan membuat sebuah data pada eloquent laravel...
```

    a.	create([
            'title' => 'Judul 1',
            'content' => 'Konten 1'
         ]);
    
    b.	Post([
            'title' => 'Judul 1',
            'content' => 'Konten 1'
         ]);
    
    **c.	Post::create([
            'title' => 'Judul 1',
            'content' => 'Konten 1'
         ]);**
    
    d.	Postcreate([
            'title' => 'Judul 1',
            'content' => 'Konten 1'
         ]);
```
    
97. setelah kita menemukan id dari data yang ingin kita rubah, kita dapat memasukan sebuah code ... untuk mengubah data dari id tersebut
```

    **a.	Post->update([
            'title' => 'Judul Satu',
            'content' => 'Konten Satu'
         ]);**
    
    b.	Post([
            'title' => 'Judul Satu',
            'content' => 'Konten Satu'
         ]);
    
    c.	update([
            'title' => 'Judul Satu',
            'content' => 'Konten Satu'
         ]);
    
    d.	Postupdate([
            'title' => 'Judul Satu',
            'content' => 'Konten Satu'
         ]);
```
   
98. setelah kita menemukan id dari data yang ingin kita hapus, kita dapat memasukan sebuah code ... untuk menghapus data dari id tersebut
```

    **a.	Post->delete();**
    
    b.	Post();
    
    c.	delete();
    
    d.	Postdelete();
```

## Mencari Mengurutkan dan Mengambil Sebagian Data
99. pada materi Mencari Mengurutkan dan Mengambil Sebagian Data, kita bisa mengambil data dengan kondisi tertentu secara spesifik menggunakan...

    a.	Post::get('is_published', true)->get();
    
    b.	Post::update('is_published', true)->get();
    
    c.	Post::delete('is_published', true)->get();
    
    **d.	Post::where('is_published', true)->get();**
    
100. kita bisa mengurutkan data secara ascending dengan menggunakan code...

    a.	Post::orderBy('id', 'desc')->get();
    
    **b.	Post::orderBy('id', 'asc')->get();**
    
    c.	Post::order('id', 'asc')->get();
    
    d.	PostorderBy('id', 'asc')->get();
    
101. kita bisa mengurutkan data secara descending dengan menggunakan code...

    **a.	Post::orderBy('id', 'desc')->get();**
    
    b.	Post::orderBy('id', 'asc')->get();
    
    c.	Post::order('id', 'asc')->get();
    
    d.	PostorderBy('id', 'asc')->get();
    
## Bekerja dengan Data Tanggal dan Waktu
102. dalam memanipulasi dateTime, laravel memakai sebuah API yang dapat melakukannya yaitu...

    a.	wood
    
    **b.	carbon**
    
    c.	steel
    
    d.	zinc
    
103. pada carbon terdapat sebuah method yang dapat mempermudah manusia dalam melihat dateTime yang sudah berapa lama sebuah data dibuat atau di rubah, yaitu method...

    a.	diffAsCarbonInterval()
    
    b.	diff()
    
    c.	diffInMonths()
    
    **d.	diffForHumans()**
    
104. kita bisa merubah sebuah data agar dapat kita manipulasi menggunakan carbon dengan menggunakan property...

    a.	$table
    
    **b.	$dates**
    
    c.	$fillable
    
    d.	semua salah

## Mengakses Properti pada Eloquent Model
105. pada model default yang ada di laravel yaitu model User.php, terdapat sebuah property $hidden yang berfungsi...

    a.	untuk menampilkan data yang di inginkan pada response
    
    **b.	untuk tidak menampilkan data yang di inginkan pada response**
    
    c.	untuk menghapus data yang di inginkan pada response
    
    d.	semua salah
    
106. contoh code pada model untuk mengakses sebuah data pada database...

    **a.	public function getUserName(){
            return $this->username;
         }**
    
    b.	public getUserName(){
            return $this->username;
         }
    
    c.	function getUserName(){
            return $this->username;
         }
    
    d.	public function getUserName(){
            return username;
         }
    
107. contoh code pada model untuk mengakses beberapa data pada database...

    **a.	public function getFullName(){
            return $this->fisrt_name . ' ' . $this->last_name;
         }**
    
    b.	public getFullName(){
            return $this->fisrt_name . ' ' . $this->last_name;
         }
    
    c.	function getFullName(){
            return $this->fisrt_name . ' ' . $this->last_name;
         }
    
    d.	public function getFullName(){
            return fisrt_name . ' ' . last_name;
         }
    
## Menggunakan Fitur Scope
108. pada materi Menggunakan Fitur Scope, penulisan function scope pada model di laravel...

    a.	public scopeActive($query){
            return $query->where('active', true);
         }
    
    b.	public function scopeActive(){
            return $query->where('active', true);
         }
    
    **c.	public function scopeActive($query){
            return $query->where('active', true);
         }**
    
    d.	public function scope Active($query){
            return $query->where('active', true);
         }
    
109. saat kita mengubah nama dari sebuah kolom di tabel database, jika kita menggunakan fitur scope maka kita hanya perlu mengubah nama dari kolom tersebut di...

    a.	controller
    
    **b.	model**
    
    c.	middleware
    
    d.	route
    
110. pada materi Menggunakan Fitur Scope, contoh penulisan code pemanggilan scope pada controller di laravel...

    **a.	$user = User::active()->get();**
    
    b.	$user = active()->get();
    
    c.	$user = Useractive()->get();
    
    d.	$user = user::active()->get();
    
111. pada materi Menggunakan Fitur Scope, contoh penulisan code pemanggilan 2 method scope pada controller di laravel...

    **a.	$user = User::active()->ageGreaterThan(20)->get();**
    
    b.	$user = active()->ageGreaterThan(20)->get();
    
    c.	$user = Useractive()->ageGreaterThan(20)->get();
    
    d.	$user = user::active()->ageGreaterThan(20)->get();
    
## Route Model Binding
112. apa yang dimaksud dengan route model binding pada laravel...

    a.	sebuah fitur yang dapat membinding controller ke sebuah model
    
    **b.	sebuah fitur yang dapat membinding route ke sebuah model**
    
    c.	sebuah fitur yang dapat membinding route ke sebuah controller
    
    d.	semua salah
    
113. pada materi Route Model Binding, penulisan function route binding pada controller di laravel...

    a.	public show(User $user){
            dd($user);
         }
    
    b.	public function show(){
            dd($user);
         }
    
    **c.	public function show(User $user){
            dd($user);
         }**
    
    d.	public function show(User){
            dd($user);
         }
    
114. pada materi Route Model Binding, penulisan function route binding pada model agar kita dapat mengambil parameter berdasarkan username di laravel...

    a.	public getRouteKeyName(){
            return 'username';
         }
    
    **b.	public function getRouteKeyName(){
            return 'username';
         }**
    
    c.	public function get RouteKeyName(){
            return 'username';
         }
    
    d.	public function get(){
            return 'username';
         }
    
115.  pada materi Route Model Binding, kita bisa menampilkan data yang sudah di activated saja dengan menambahkan sebuah kondisi di sebuah file...

    a.	AppServiceProvider.php
    
    b.	AuthServiceProvider.php
    
    c.	EventServiceProvider.php
    
    **d.	RouteServiceProvider.php**
    
