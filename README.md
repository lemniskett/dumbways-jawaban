# 1

Dev Ops adalah sebuah set praktik dan para pengembang yang bekerja sama untuk men-*support* sebuah layanan, dimulai dari selama pengembangan sampai ke bagian *production*.

Tanpa Dev Ops, akan lebih banyak tekanan yang akan di-*handle* para programmer, dan *potentially* staff lain.

Flow dari development ke production

![01](/images/01.png)

# 2

Docker adalah sebuah container yang fungsi utamanya untuk menge-*ship* sebuah software tanpa perlu memikirkan dependensi, semua dependensi software di-*bundle* menjadi sebuah *image* dan *image* ini bisa di-transfer ke host apapun tanpa menginstall dependensi di host tersebut, mirip seperti virtual machine namun host dan guest docker menggunakan kernel yang sama (dan *optionally* resource lain yang sama), jauh lebih sedikit *overhead*-nya dibandingkan virtual machine. Sedangkan Kubernetes adalah container manager, Kubernetes seperti layaknya orkestra yang memandu container-container yang di-*manage*, Kubernetes dapat mengatur *scale*, *deploy* otomatis, dan mengatur container-container.

Berikut adalah struktur docker :

![02-step-1](/images/02-step-1.png)

Berikut adalah struktur kubernetes, simplified :

![02-step-2](/images/02-step-2.png)

perbedaannya adalah docker adalah *container*, sedangkan Kubernetes adalah manajer dari kumpulan-kumpulan *container*,
sedangkan persamaannya adalah keduanya merupakan solusi untuk memudahkan deployment.

# 3

Untuk mencari sebuah command yang pernah dijalankan, kita bisa menggunakan Tombol up untuk menampilkan command sebelumnya.

Sebelum tombol up:

![03-step-1](/images/03-step-1.png)

Setelah tombol up:

![03-step-2](/images/03-step-2.png)

Kita juga bisa melihat histori command yang pernah dijalankan, umumnya file histori terletak pada $HOME/.bash_history (dimana ```$HOME``` adalah ```/home/<nama user>``` bagi user biasa dan ```/root``` bagi root user) bila menggunakan shell bash, untuk melihatnya kita bisa execute command ```cat ~/.bash_history``` atau ```less ~/.bash_history``` :

![03-step-3](/images/03-step-3.png)

![03-step-4](/images/03-step-4.png)

![03-step-5](/images/03-step-5.png)

Untuk mencari command di histori, execute command ```grep "$search" ~/.bash_history``` (dimana ```$search``` merupakan apa yang kita ingin cari) :

![03-step-6](/images/03-step-6.png)

# 4

Dengan CI (*Continuous Integration*), setiap ada *changes*, akan ada *automated* build. bila ada kesalahan, dapat terdeteksi dengan mudah dimana dan apa yang salah.
Dengan CD, *changes* dapat sampai ke *production* dengan lebih cepat dan aman dengan mengecek apakah itu deployable atau tidak.

![04](/images/04.png)

# 5

[Video link](/videos/05.mp4)

# 6

[Video link](/videos/06.mp4)

# 8

Untuk database, saya akan menggunakan layanan remotemysql.com karena saya tidak punya credit card untuk menggunakan ClearDB

## Create project di Heroku

![08-step-1](/images/08-step-1.png)

## Set environment variables untuk MySQL

![08-step-2](/images/08-step-2.png)

## Initialize Git repository

Buat sebuah directory bernama lemniskett-wp, cd ke dir tersebut, buat repo git, dan tambahkan remote heroku

![08-step-3](/images/08-step-3.png)

## Set up webserver

![08-step-4](/images/08-step-4.png)

## Buat composer.json untuk installasi dependensi

![08-step-5](/images/08-step-5.png)

## Tambahkan /vendor ke dalam gitignore, dan lakukan composer update

![08-step-6](/images/08-step-6.png)

![08-step-7](/images/08-step-7.png)

## Download latest wordpress release tarball

![08-step-8](/images/08-step-8.png)

## Extract dan hapus tarball-nya

![08-step-9](/images/08-step-9.png)

## Push ke remote heroku

![08-step-10](/images/08-step-10.png)

![08-step-11](/images/08-step-11.png)

## Missing procfile dan composer.json, git add . di root repo, git commit, dan push ke remote heroku

![08-step-12](/images/08-step-12.png)

## Wordpress initial setup

![08-step-13](/images/08-step-13.png)

## Wordpress initial setup

![08-step-14](/images/08-step-14.png)

## Done

Username : lemniskett
Password : dumbways

![08-step-15](/images/08-step-15.png)
