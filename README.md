<b> Nama : Diana Dwi Rahayu
<p> NIM : 312010055
<p> Kelas : TI.20.D1
<p> Mata Kuliah : Sistem Basis Data
<p> Pertanyaan dan Tugas </b>
<p> 1. Masuk database dengan nama_nim

![1](https://user-images.githubusercontent.com/101866805/171573840-7f54ba26-7122-46f7-88f1-f4ba322d2c63.png)
<p> 2. Lakukan proses backup dan recovery dengan sql dari database tugas sebelumnya
<p> a. Proses Backup
<p> Melakukan proses penguncian/lock table

![2](https://user-images.githubusercontent.com/101866805/171570476-6319a8ee-1595-41e3-a963-82beca37b61f.png)
<p> Lakukan proses backup table dengan perintah : SELECT * INTO OUTFILE

![3](https://user-images.githubusercontent.com/101866805/171570669-6c2f3a7e-0206-431b-8c4f-f5d275365071.png)
<p> Untuk mengecek hasil backup, dapat dibuktikan file backup ada pada direktori C:\xampp\mysql\data\dianadwirahayu_312010055

![4](https://user-images.githubusercontent.com/101866805/171570930-f2182278-6c33-4b65-b99d-cca4d22bac25.png)
<p> b. Proses Recovery/Restore
<p> Untuk membuktikan bahwa proses berhasil yaitu menghapus tabel mahasiswa_312010055, kemudian lihat hasilnya jikas sudah kosong berarti proses hapus berhasil
<p> Kemudian lakukan recovery dengan sql seperti berikut

![5](https://user-images.githubusercontent.com/101866805/171571251-e3bcbb35-4cd3-4c65-b979-1e7d46236dc4.png)
<p> 3. Lakukan proses backup dan recovery dengan sqldump dari database tugas sebelumnya
<p> a. Jalankan shell atau command-prompt dan ketikkan perintah berikut untuk memulai dump database mysqldump –u root –p dianadwirahayu_312010055 > mahasiswa_312010055.sql

![6](https://user-images.githubusercontent.com/101866805/171572807-a7e23867-624a-4400-b44a-89f29d6880cf.png)
<p> b. Data yang telah di backup dapat di restrore kembali ke dalam database dengan perintah mysqldump -u root -p dianadwirahayu_312010055 < c:\xampp\mysql\bin\mahasiswa_312010055.sql

![7](https://user-images.githubusercontent.com/101866805/171573149-5ef9e5db-93ae-42b8-afa4-61fb1be25756.png)
![8](https://user-images.githubusercontent.com/101866805/171573183-d1f54f09-9cf8-44c8-bdb4-1061b5638516.png)
<p> 4. Tuliskan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam
<p> 0 0 * * 7
