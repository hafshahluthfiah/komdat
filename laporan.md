# Aplikasi Web "PHPBack"

> Shita Maharani (G64140037), Selfi Qisthina (G64140059), Hafshah Luthfiah (G64140096)

## Sekilas Tentang

PHPBack adalah sebuah aplikasi web yang dibuat dengan PHP/MySQL yang memungkinkan pengguna untuk membagikan suatu ide dan mendapat feedback dari user lain mengenai ide tersebut. 


## Instalasi
#### Kebutuhan
- Apache 2.2+ atau Nginx
- MySQL Server 4.1+
- PHP versi 5.3+


#### Cara instalasi
1. Unduh arsip ZIP instalasi PHPBack dan simpan ke dalam direktori var/www/html/. 
	```bash
	$ mkdir var/www/html/
	$ cd var/www/html/
	$ wget http://www.phpback.org/files/phpback_v1.3.1.zip
	```

2. *Unzip* arsip yang sudah terunduh. 
``$ unzip phpback_v1.3.1.zip``


3. Selanjutnya buka http://localhost (localhost -> alamat IP atau URL kamu). Selanjutnya ikuti langkah-langkah untuk konfigurasi.
	- Konfigurasi database
	
	![](https://1.bp.blogspot.com/-e4NhG_YHubQ/WNPYTxYAV9I/AAAAAAAAAj8/TtWmV_9XqfgcDdqTa-m1JHRp-_KXX0GpQCLcB/s1600/4.PNG)
	
	- Menghapus file 
		```bash
		$ cd install
		$ rm index.php
		$ rm install1.php
		$ rm database_tables.sql
		```
	
    	![](https://3.bp.blogspot.com/-zwjC4EI3qfA/WNPb5LBJ56I/AAAAAAAAAkU/EQ71sIlWgBYLxMC0RDcojgTufi8Wcv8BwCLcB/s1600/7.PNG)
	
	- Pengaturan akun admin
	
	![](https://4.bp.blogspot.com/-8ZAN6X2wRT8/WNPYT_5_VSI/AAAAAAAAAj0/ZI6uW9tuPOcQM2vvCGROIWy0Yjr4pu_7ACLcB/s1600/5.PNG)
    
	- Pengaturan user management
	
	![](https://2.bp.blogspot.com/-Zr_pa3R59NA/WNPYUSBMuBI/AAAAAAAAAkE/ATU_ZQUlbJAoWodIyUQXeZQnnO4vq38vwCLcB/s1600/8.PNG)
	
	- Menghapus direktori 
	``$ rm -d install``
-	
    	![](https://3.bp.blogspot.com/-nrzRq5wXwTo/WNPbLXY-nqI/AAAAAAAAAkQ/SmRBQzUBUv8XHogVp_CVk1Kqg7gYtFBdACLcB/s1600/7.PNG)
    
	- Login admin
	
    	![](https://1.bp.blogspot.com/-Arvn-7yc5hg/WNPbBpHo9UI/AAAAAAAAAkM/aevfIE0i8BE7StcCznI2cUZCVIKWVwpAACLcB/s1600/8_baru.PNG)
	
	- Selesai. (Masuk ke halaman admin)
	
    	![](https://4.bp.blogspot.com/-ebEDcoHXrvI/WNPbBoaGY9I/AAAAAAAAAkI/mOSqSaWKs-g2jreWiDODV3STEaEZ8ySkgCLcB/s1600/9_baru.PNG)


## Konfigurasi (opsional)

- Pastikan pada konfigurasi Apache, *module* ``mod_rewrite`` sudah dalam keadaan aktif. Untuk melihat *module* mana yang sudah aktif, ketikkan perintah ``apache2ctl -M``.  Jika belum ada di *list*, ketikkan perintah ``sudo a2enmod rewrite`` pada terminal kemudian *restart* apache dengan mengetikkan perintah ``sudo service apache2 restart``. 
- Mengubah permission agar data dapat diakses di internet ``$ chown –R www–data:www-data *``

## Otomatisasi

(**_tidak ada_**)


## Cara Pemakaian

- Fungsi-fungsi utama user
	- Register
	
	![](https://2.bp.blogspot.com/-K8sM7LndE84/WNPoEX5dQjI/AAAAAAAAAk0/ZUkoHD67utI6hF7vXE0z2L3Yfb2PdE06gCLcB/s1600/13.PNG)
	
	- Login
	
	![](https://hafshahluthfiah.files.wordpress.com/2017/03/login1.jpg)
	
	- Memposting idea
	
	![](https://3.bp.blogspot.com/-KDdDsJ0rl2o/WNPoEFBF31I/AAAAAAAAAkw/Pmo3sv-t1fIzktYoEJF3S7PeqFq6AWedACLcB/s1600/14.PNG)
	
- Fungsi-fungsi utama admin
	- Approve/Delete idea dan Ban User
	
	![](https://4.bp.blogspot.com/-_5oyvMoMJQA/WNPm144HwFI/AAAAAAAAAkk/6MAO8bP-ISEvLoo-jAul7r8lTQS3JJuGACLcB/s1600/10.PNG)
	
	- User management
	
	![](https://2.bp.blogspot.com/-42q-NwmIeA0/WNPm2ODOpHI/AAAAAAAAAko/n5nnO16XURUtft9jk94MrDAZcANR9WtzACLcB/s1600/12.PNG)


## Pembahasan

- Pendapat tentang aplikasi web ini
	- Pros:
		- Situs PHPback merupakan sebuah aplikasi berbasis web yang sangat bermanfaat terutama untuk web developper. Dengan adanya PHPback, orang-orang dapat saling membantu satu sama lain dalam bertukar idea mengenai developping system. PHPback ini merupakan salah satu fasilitas untuk mencerdaskan komunitas-komunitas web developper di seluruh dunia. Keunggulan PHPback diantaranya adalah sangat responsive karena sistem dibangun dengan framework bootstrap. PHPBack dibuat dengan CodeIgniter Framework, sehingga para php developper dapat dengan mudah untuk memahami dan mengedit code.
		
	- Cons:
		- Tidak ada validasi email ketika mengisi form registrasi user, sehingga orang dapat mengisi field email dengan email palsu dan melakukan spamming pada akun PHPback anda.
		
- Perbandingan dengan aplikasi web sejenis
	- UserVoice
		UserVoice merupakan sebuah aplikasi berbasis web dimana seorang developer atau sebuah perusahaan dapat berbagi ide nya atau feedback dari customer. beberapa fiturnya adalah sharing ideas, voting ide terbaik dan membuat forum. Perbedaan UserVoice dengan PHPBack yaitu phpback merupakan opensource sedangkan uservoice bersifat berbayar dan terbilang cukup mahal yang dapat menyebabkan projek-projek kecil atau pun perusahaan kecil susah untuk menjangkau UserVoice.


## Referensi

https://github.com/ivandiazwm/phpback
https://github.com/ivandiazwm/phpback/wiki/How-To-install

