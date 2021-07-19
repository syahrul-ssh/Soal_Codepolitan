# Pendahuluan
## Installasi Laratrust
1.  Sebuah package yang memudahkan untuk mengimplementasikan role dan permission pada laravel, adalah pengertian dari...

    a.  Laracast
    
    b.  Laragon
    
    **c.  Laratrust**
    
    d.  semua salah

2.  Versi terbaru dari Laratrust saat ini adalah...

    a.  4.0
    
    b.  5.2
    
    c.  5.1
    
    **d.  6.x**

3.  Dibawah ini adalah beberapa hal yang di support oleh laratrust, kecuali...

    a.  Multiple user models.
    
    b.  Roles and permissions verification.
    
    **c.  Make a good view template to user**
    
    d.  Objects ownership verification.
    
4.  Berikut cara untuk menginstall package laratrust pada project laravel...

    **a. composer require santigarcor/laratrust**
    
    b.  composer santigarcor/laratrust
    
    c.  composer require laratrust
    
    d.  semua salah

5.  berdasarkan materi Installasi Laratrust, kita melakukan konfigurasi di file AppServiceProvider.php pada fungsi register, kita menambahkan sebuah code berikut...

    a.  Schema::StringLength(191);
    
    **b.  Schema::defaultStringLength(191);**
    
    c.  defaultStringLength(191);
    
    d.  Schema::defaultLength(191);

6.  Setelah kita melakukan Installasi Laratrust kita perlu untuk melakukan publish konfigurasi dari laratrust itu sendiri dengan melakukan perintah...

    **a. php artisan vendor:publish --tag="laratrust"**
    
    b.  php vendor:publish --tag="laratrust"
    
    c.  php artisan vendor:publish "laratrust"
    
    d.  php artisan publish --tag="laratrust"
    
7.  Setelah kita melakukan publishing pada installasi laratrust, selanjutnya kita perlu melakukan setup laratrust dengan melakukan perintah...

    a.  php artisan setup
    
    b.  php artisan laratrust
    
    **c.  php artisan laratrust:setup**
    
    d.  php laratrust:setup
    
8.  Sebelum kita melakukan migrate ke database, kita bisa membuat dump data menggunakan seeder untuk role dan permission menggunakan perintah...

    **a.  php artisan laratrust:seeder**
    
    b.  php artisan laratrust
    
    c.  php laratrust:seeder
    
    d.  php artisan seeder
    
9.  Setelah kita menjalankan perintah untuk melakukan dump data selanjutnya kita harus memanggil class LaratrustSeeder nya di DatabaseSeeder menggunakan sebuah code berukut...

    a.  $this->(LaratrustSeeder::class);
    
    b.  call(LaratrustSeeder::class);
    
    c.  $this->call(Laratrust::class);
    
    **d.  $this->call(LaratrustSeeder::class);**

## Membuat Model Article beserta Factory
10. Berdasarkan materi Membuat Model Article beserta Factory, kita membuat sebuah model untuk artikel menggunakan perintah artisan sebagai berikut...

    a.  php make:model Article -mfs
    
    **b.  php artisan make:model Article -mfs**
    
    c.  php artisan model Article -mfs
    
    d.  php artisan make:model Article

11. Berdasarkan materi Membuat Model Article beserta Factory, Pada file migration yang telah dibuat kita melakukan konfigurasi field apa saja yang akan kita buat pada table databasenya, berikut beberapa field yang dibuat, kecuali...

    a.  published
    
    b.  title
    
    c.  body
    
    **d.  user**

12. Berdasarkan materi Membuat Model Article beserta Factory, lengkapilah potongan code yang ada di ArticleFactory.php berikut 'title' => $...->sentence(4)

    a.  call
    
    b.  factory
    
    **c.  faker**
    
    d.  semua salah
    
13. Berdasarkan materi Membuat Model Article beserta Factory, lengkapilah potongan code yang ada di ArticleSeeder.php berikut ...(Article::class, 20)->create();

    a.  call
    
    **b.  factory**
    
    c.  faker
    
    d.  semua salah

14. Berdasarkan materi Membuat Model Article beserta Factory, lengkapilah potongan code yang ada di DatabaseSeeder.php berikut $this->...(ArticleSeeder::class);

    **a.  call**
    
    b.  factory
    
    c.  faker
    
    d.  semua salah

15. Berdasarkan materi Membuat Model Article beserta Factory, lengkapilah potongan code yang ada di Article.php berikut return $this->...(User::class);

    a. belongstoMany
    
    b.  belongs
    
    c.  hasMany
    
    **d.  belongsTo**
    
16. Berdasarkan materi Membuat Model Article beserta Factory, lengkapilah potongan code yang ada di User.php berikut return $this->...(Article::class);

    a. belongsToMany
    
    b.  belongs
    
    **c.  hasMany**
    
    d.  belongsTo
    
