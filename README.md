# SIUNIVmodul7
![alt text](https://github.com/adristiputri/SIUNIVmodul7/blob/master/Screenshot%20(149).png)
![alt text](https://github.com/adristiputri/SIUNIVmodul7/blob/master/Screenshot%20(150).png)
![alt text](https://github.com/adristiputri/SIUNIVmodul7/blob/master/Screenshot%20(152).png)
![alt text](https://github.com/adristiputri/SIUNIVmodul7/blob/master/Screenshot%20(153).png)
1.Berikan contoh kode keneksi untuk ke database pd php
<?php
$servername = "localhost";
$database = "niagahos_namadatabase";
$username = "niagahos_user";
$password = "passworddatabase";

// untuk tulisan bercetak tebal silakan sesuaikan dengan detail database Anda
// membuat koneksi
$conn = mysqli_connect($servername, $username, $password, $database);
// mengecek koneksi
if (!$conn) {
    die("Koneksi gagal: " . mysqli_connect_error());
}
echo "Koneksi berhasil";
mysqli_close($conn);
?>

2.Bagaimana cara anda membuat database pada phpMySQl!
 1.Menjalankan APACHE dan MYSQL dalam status RUN 
 2.Ketik http://localhost/phpmyadmin 
 3.Pada menu Database, silahkan masukkan nama database yang diinginkan, kemudian klik Create. 
 4.Setelah di create sekarang kita akan membuat table pada database tersebut. masukkan nama table yang anda inginkan, lalu masukkan jumlah kolom yang ingin anda buat. Lalu klik GO 
 5.Pada langkah ini kita akan memasukkan nama kolom yang ingin kita masukkan, misal pada artikel kali ini kita akan membuat field untuk ID, NAMA, ALAMAT 6.Jika sudah terisi field-field yang di perlukan, sekarang klik SAVE pada pojok kanan bawah. 
 
3.Berikan code query untuk menampilkan sebuah data yang ada pada ke database?
SELECT apa_yang_akan_ditampilkan FROM tabel_apa WHERE kondisi_apa_data_ditampilkan;

4. Berikan code query untuk mengupdate sebuah data yang ada pada ke database?
UPDATE pelanggan SET nama_pelanggan = 'John Doe';

5. Berikan code query untuk menghapus sebuah data yang ada pada ke database?
DELETE FROM karyawan WHERE id_karyawan= '1';
