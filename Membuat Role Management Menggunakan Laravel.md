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
    
# Membuat Role Management
## Membuat Component Blade Alert
17. Berikut adalah contoh perintah artisan untuk membuat component alert...

    a.  php make:component Alert
    
    **b.  php artisan make:component Alert**
    
    c.  artisan make:component Alert
    
    d.  php artisan component Alert

18. Pada file alert.php yang telah kita buat menggunakan perintah artisan didalamnya kita menambahkan public property berikut...

    **a.  $type & $message**
    
    b.  $get & $post
    
    c.  $guarded
    
    d.  semua salah

19. Berdasarkan materi Membuat Component Blade Alert, pada file alert.php lengkapilah potongan code berikut $this->... = $type;

    a.  tipe
    
    **b.  type**
    
    c.  message
    
    d.  view
    
20. Berdasarkan materi Membuat Component Blade Alert, pada file alert.php lengkapilah potongan code berikut $this->... = $message;

    a.  tipe
    
    b.  type
    
    **c.  message**
    
    d.  view

21. Berdasarkan materi Membuat Component Blade Alert, pada file alert.php lengkapilah potongan code berikut return ...('components.alert');

    a.  tipe
    
    b.  type
    
    c.  message
    
    **d.  view**

22. Berdasarkan materi Membuat Component Blade Alert, pada folder app kita membuat sebuah folder baru yang bernama Traits, di dalam folder Traits kita membuat sebuah file...

    a.  flashAlert.php
    
    b.  Flashalert.php
    
    **c.  FlashAlert.php**
    
    d.  flashalert.php
    
23. Dibawah ini adalah beberapa method yang di buat di dalam file FlashAlert.php...

    a.  alertDeleted()
    
    b.  alertCreated()
    
    c.  alertUpdated()
    
    **d.  semua benar**
    
## Membuat CRUD User
24. Dibawah ini perintah untuk mengenerate UserController berdasarkan materi dari Membuat CRUD User...

    a.  php artisan make:controller UserController --resource
    
    b.  php artisan make:controller Admin/UserController
    
    **c.  php artisan make:controller Admin/UserController --resource**
    
    d.  php artisan controller Admin/UserController --resource

25. Pada file bernama UserController.php tepatnya pada method index, lengkapilah potongan code berikut $users = User::...(10);

    a.  pagination
    
    **b.  paginate**
    
    c.  paginates
    
    d.  paginet

26. Berdasarkan materi Membuat CRUD User, Pada file bernama index.blade.php, lengkapilah potongan code berikut `<... :type="session('type')" :message="session('message')"/>`

    a.  z-alert
    
    b.  y-alert
    
    **c.  x-alert**
    
    d.  a-alert
    
27. Berdasarkan materi Membuat CRUD User, Pada file bernama create.blade.php, lengkapilah potongan code berikut {{ $...->display_name }}

    a.  rule
    
    b.  roles
    
    **c.  role**
    
    d.  rules

28. Berdasarkan materi Membuat CRUD User, Pada file bernama edit.blade.php, lengkapilah potongan code berikut {{$...->name}}

    a.  use
    
    b.  users
    
    **c.  user**
    
    d.  used

29. Berdasarkan materi Membuat CRUD User, Pada file bernama web.php, lengkapilah potongan code berikut Route::middleware(['...', 'role:superadmin'])

    a.  semua salah
    
    b.  authenticate
    
    c.  authentication
    
    **d.  auth**
    
30. Berdasarkan materi Membuat CRUD User, Pada file bernama app.blade.php, lengkapilah potongan code berikut {{ ...('admin.user.index') }}

    a.  routes
    
    **b.  route**
    
    c.  routing
    
    d.  rotation
    
## Membuat CRUD Permission
31. Dibawah ini perintah untuk mengenerate PermissionController berdasarkan materi dari Membuat CRUD Permission...

    a.  php artisan make:controller PermissionController --resource
    
    b.  php artisan make:controller Admin/PermissionController
    
    **c.  php artisan make:controller Admin/PermissionController --resource**
    
    d.  php artisan controller Admin/PermissionController --resource

32. Pada file bernama PermissionController.php, pada method create, lengkapilah potongan code berikut return view('pages.admin. ... .create');

    a.  permit
    
    **b.  permission**
    
    c.  license
    
    d.  validate

33. Pada file bernama PermissionController.php, pada method store, lengkapilah potongan code berikut $this->...($request, []);

    a.  permit
    
    b.  permission
    
    c.  license
    
    **d.  validate**
    
34. Pada file bernama PermissionController.php, pada method edit, lengkapilah potongan code berikut $... = Permission::findOrFail($id);

    a.  permit
    
    **b.  permission**
    
    c.  license
    
    d.  validate

35. Berdasarkan materi Membuat CRUD Permission, Pada file bernama index.blade.php, lengkapilah potongan code berikut {{ ...('admin.permission.create') }}

    a.  routes
    
    **b.  route**
    
    c.  routing
    
    d.  rotation

36. Berdasarkan materi Membuat CRUD Permission, Pada file bernama create.blade.php, lengkapilah potongan code berikut {{ ...('name') }}

    a.  teen
    
    b.  young
    
    **c.  old**
    
    d.  kid
    
37. Berdasarkan materi Membuat CRUD Permission, Pada file bernama web.php, lengkapilah potongan code berikut Route::...('permission', 'PermissionController');

    a.  source
    
    b.  resources
    
    **c.  resource**
    
    d.  semua salah

## Membuat CRUD Role
38. Dibawah ini perintah untuk mengenerate RoleController berdasarkan materi dari Membuat CRUD Role...

    a.  php artisan make:controller RoleController --resource
    
    b.  php artisan make:controller Admin/RoleController
    
    **c.  php artisan make:controller Admin/RoleController --resource**
    
    d.  php artisan controller Admin/RoleController --resource

39. Berdasarkan materi Membuat CRUD Role, Pada file bernama RoleController.php, pada method store, lengkapilah potongan code berikut $role->...($request->input('permissions_id'));

    a.  permissions
    
    **b.  attachPermissions**
    
    c.  forceDelete
    
    d.  attachpermission

40. Berdasarkan materi Membuat CRUD Role, Pada file bernama RoleController.php, pada method edit, lengkapilah potongan code berikut $... = Permission::all();

    **a.  permissions**
    
    b.  attachPermissions
    
    c.  forceDelete
    
    d.  syncPermissions
    
41. Berdasarkan materi Membuat CRUD Role, Pada file bernama RoleController.php, pada method update, lengkapilah potongan code berikut $role->...($request->input('permissions_id'));

    a.  permissions
    
    b.  attachPermissions
    
    c.  forceDelete
    
    **d.  syncPermissions**

42. Berdasarkan materi Membuat CRUD Role, Pada file bernama RoleController.php, pada method destroy, lengkapilah potongan code berikut $role->...();

    a.  permissions
    
    b.  attachPermissions
    
    **c.  forceDelete**
    
    d.  syncPermissions

43. Berdasarkan materi Membuat CRUD Role, Pada file bernama web.php, lengkapilah potongan code berikut Route::resource('...', 'RoleController');

    **a.  role**
    
    b.  user
    
    c.  permission
    
    d.  article
    
## Membuat CRUD Article
44. Dibawah ini perintah untuk mengenerate ArticleController berdasarkan materi dari Membuat CRUD Article...

    **a.  php artisan make:controller ArticleController --resource**
    
    b.  php artisan make:controller Admin/ArticleController
    
    c.  php artisan make:controller Admin/ArticleController --resource
    
    d.  php artisan controller Admin/ArticleController --resource

45. Berdasarkan materi Membuat CRUD Article, Pada file bernama ArticleController.php, pada method index, lengkapilah potongan code berikut $... = Article::paginate(10);

    a.  roles
    
    b.  users
    
    c.  permissions
    
    **d.  articles**

46. Berdasarkan materi Membuat CRUD Article, Pada file bernama ArticleController.php, pada method store, lengkapilah potongan code berikut return redirect()->route('article.index')->with($this->...());

    a.  alertDeleted
    
    b.  alertUpdated
    
    **c.  alertCreated**
    
    d.  permissionDenied
    
47. Berdasarkan materi Membuat CRUD Article, Pada file bernama ArticleController.php, pada method update, lengkapilah potongan code berikut return redirect()->route('article.index')->with($this->...());

    a.  alertDeleted
    
    **b.  alertUpdated**
    
    c.  alertCreated
    
    d.  permissionDenied

48. Berdasarkan materi Membuat CRUD Article, Pada file bernama ArticleController.php, pada method destroy, lengkapilah potongan code berikut return redirect()->route('article.index')->with($this->...());

    **a.  alertDeleted**
    
    b.  alertUpdated
    
    c.  alertCreated
    
    d.  permissionDenied

49. Berdasarkan materi Membuat CRUD Article, Pada file bernama web.php, lengkapilah potongan code berikut Route::resource('...', 'ArticleController');

    a.  role
    
    b.  user
    
    c.  permission
    
    **d.  article**
    
## Implementasi Role dan Permission di Controller
50. Berdasarkan materi Implementasi Role dan Permission di Controller, Pada file bernama ArticleController.php, pada method edit, lengkapilah potongan code berikut request()->user()->hasRole(['...', 'admin'])

    **a.  superadmin**
    
    b.  admin
    
    c.  user
    
    d.  semua salah

51. Berdasarkan materi Implementasi Role dan Permission di Controller, Pada file bernama ArticleController.php, pada method edit, lengkapilah potongan code berikut request()->user()->isAbleToAndOwns('...', $article)

    a.  articles-update
    
    b.  delete-articles
    
    **c.  update-articles**
    
    d.  articles

52. Berdasarkan materi Implementasi Role dan Permission di Controller, Pada file bernama ArticleController.php, pada method destroy, lengkapilah potongan code berikut request()->user()->hasRole('...')

    **a.  superadmin**
    
    b.  admin
    
    c.  user
    
    d.  semua salah

53. Berdasarkan materi Implementasi Role dan Permission di Controller, Pada file bernama ArticleController.php, pada method destroy, lengkapilah potongan code berikut request()->user()->isAbleToAndOwns('...', $article)

    a.  articles-update
    
    **b.  delete-articles**
    
    c.  update-articles
    
    d.  articles

54. Berdasarkan materi Implementasi Role dan Permission di Controller, Pada file bernama index.blade.php, yang ada di folder view article, lengkapilah potongan code berikut {{ $article->user->... }}

    a.  names
    
    **b.  name**
    
    c.  nama
    
    d.  semua salah

55. Ketika kita login sebagai user, pesan apa yang akan ditampilkan apabila kita berusaha mengedit atau menghapus artikel yang kita tidak memiliki permissionnya...

    a.  Something wrong!
    
    **b.  you don’t have permission to access!**
    
    c.  Data successfully updated!
    
    d.  Data not found!
    
## Implementasi Role dan Permission di Blade
56. Berdasarkan materi Implementasi Role dan Permission di Blade, Kita dapat menghilangkan menu user, permission, dan role pada file blade, tepatnya pada file...

    **a.  app.blade.php**
    
    b.  index.blade.php
    
    c.  menu.blade.php
    
    d.  nav.blade.php

57. Berdasarkan materi Implementasi Role dan Permission di Blade, Kita dapat menghilangkan menu user, permission, dan role pada file blade, dengan menambahkan method menggunakan syntax blade, berikut methodnya...

    **a.  @role()**
    
    b.  @roles()
    
    c.  @rules()
    
    d.  @rule()

58. Berdasarkan materi Implementasi Role dan Permission di Blade, Pada file bernama edit.blade.php, yang ada di folder view article, lengkapilah potongan code berikut ...(['superadmin', 'admin'])

    a.  @rules
    
    b.  @roles
    
    c.  @rule
    
    **d.  @role**
    
59. Apa nilai default dari data published yang dibuat pada course ini...

    a.  true
    
    **b.  false**

60. Ketika kita login sebagai user, pesan apa yang akan ditampilkan apabila kita sudah mengedit article yang kita sebagai user buat...

    a.  Something wrong!
    
    b.  you don’t have permission to access!
    
    **c.  Data successfully updated!**
    
    d.  Data not found!
    
