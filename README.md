# arsipdatasiswa
Repository Untuk Melaporkan Bug Software

Script Aplikasi Arsip Data Siswa,

Tutorial Cara Menginstall :

Aplikasi ini bisa digunakan di server lokal, maupun di hostingkan secara online.

A. Tutorial Menginstall di Server Lokal
* Pastikan Anda Menggunakan Server Lokal XAMPP
PHP version: 5.6.31 (Versi 7 Tidak Apa) dan Mysql 10.1.25-MariaDB

	1. Copy Semua File Kedalam c:\xampp\htdocs\namafile
		(Ubah 'namafile' sesuai keinginan kamu)
	2. Setelah semua siap di copy, edit database nya di file application/config/database.php

	Ubah Yang Di Bagian : 

	 $db['default'] = array(
	'dsn'	=> '',
	'hostname' => 'localhost', 
	'username' => 'root', <-- User Database Anda
	'password' => '', <-- Password Database Anda (Kosongkan Jika Tidak Ada)
	'database' => 'arsip', <-- nama database di phpmyadmin
	'dbdriver' => 'mysqli',
	'dbprefix' => '',
	'pconnect' => FALSE,
	'db_debug' => (ENVIRONMENT !== 'production'),
	'cache_on' => FALSE,
	'cachedir' => '',
	'char_set' => 'utf8',
	'dbcollat' => 'utf8_general_ci',
	'swap_pre' => '',
	'encrypt' => FALSE,
	'compress' => FALSE,
	'stricton' => FALSE,
	'failover' => array(),
	'save_queries' => TRUE();

	Yang Lain Tidak Diubah

	3. Terakhir , Impor Data Mysql Di Folder backup_sql

	Setalah Itu Jalankan, Untuk Default Login :
	Administrator :
	User : admin
	Pass : admin

	Staff :
	user : pegawai
	pass : whoami2002

<!---------------------------------------------------------------------------------------------------->

B. Tutorial Menginstall di Hosting


	1. Upload Semua File Kedalam file manager cpanel  /home/user/public_html
		(nama 'user' sesuai dengan username cpanel)
	2. Setelah semua siap di copy, edit database nya di file application/config/database.php

	Ubah Yang Di Bagian : 

	 $db['default'] = array(
	'dsn'	=> '',
	'hostname' => 'localhost', 
	'username' => 'root', <-- User Database Anda
	'password' => '', <-- Password Database Anda (Kosongkan Jika Tidak Ada)
	'database' => 'arsip', <-- nama database di phpmyadmin
	'dbdriver' => 'mysqli',
	'dbprefix' => '',
	'pconnect' => FALSE,
	'db_debug' => (ENVIRONMENT !== 'production'),
	'cache_on' => FALSE,
	'cachedir' => '',
	'char_set' => 'utf8',
	'dbcollat' => 'utf8_general_ci',
	'swap_pre' => '',
	'encrypt' => FALSE,
	'compress' => FALSE,
	'stricton' => FALSE,
	'failover' => array(),
	'save_queries' => TRUE();

	Yang Lain Tidak Diubah

	3. Terakhir , Impor Data Mysql Di Folder backup_sql

	Setalah Itu Jalankan, Untuk Default Login :
	Administrator :
	User : admin
	Pass : admin

	Staff :
	user : pegawai
	pass : whoami2002


Untuk Mengimport data siswa dengan file .csv, silahkan lihat template 
di folder "Format Import Siswa"

jika ingin mengubah title, footer, logo , dll bisa diedit di

1. folder /views
2. folder /application/controllers/

Sekian Tatacara Konfigurasinya, Jika Ingin Menanyakan cara lainya silahkan kontak :

FB : fb.com/rifky.host
Line : dev_ky
Email : saya@rifky.tech
