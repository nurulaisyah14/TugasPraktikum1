# TugasPraktikum1
# Tugas Praktikum { Pertemuan ke 6 } <img src=https://qph.fs.quoracdn.net/main-qimg-648763cc041459725b62108f4fdf5b91 width="110px" >
|**Nama**|**NIM**|**Kelas**|**Mata kuliah**|**Dosen Pengampu**|
|----|---|-----|------|---------|
|Nurul Aisyah|312310476|TI.23.A5|Basis Data|Agung Nugroho, S.Kom., M.Kom|


## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Latihan Praktikum1|[Click Here](#Latihan-Praktikum1)|
|1|Pengertian INT|[Click Here](#Pengertian-INT)|
|2|Penjelasan Kolom DESC|[Click Here](#Penjelasan-Kolom-DESC)|

# Latihan Praktikum1
## 1. Tulis semua perintah-perintah SQL percobaan di atas beserta outputnya!

**1. Buat sebuah database dengan nama latihan2**

Untuk membuat database gunakan perintah sebagai berikut :

`CREATE DATABASE [nama_database]`

`CREATE DATABASE latihan2;`

lalu, setelah kita membuat database. kita masuk kedalam database tersebut dengan perintah sebagai berikut :

`USE latihan2;`

![alt text](![Screenshot 2024-04-23 090357](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/64ae7bff-2316-4f8e-be58-cc5b80fa9b73)
)

**2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!**

Untuk membuat Tabel gunakan perintah sebagai berikut :

`CREATE TABLE nama_tabel (
    nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran)
    );`

`CREATE TABLE biodata (
    nama varchar (100),
    alamat text
    );`

![alt text](![Screenshot 2024-04-23 184135](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/3e41c110-b33c-4711-9dbd-97458e4058b5)
)

**3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!**

Contoh :

`ALTER TABLE biodata ADD COLUMN keterangan VARCHAR (15);`

![alt text](![Screenshot 2024-04-23 184152](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/37137a18-7491-4f4b-9ef9-c313a15bec65)
)

**4.Tambahkan kolom id(int 11) di awal (sebagai kolom pertama)!**

Untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut :

`ALTER TABLE biodata ADD COLUMN id int FIRST; `

![alt text](![Screenshot 2024-04-23 184202](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/5e19eec7-1e20-4645-80d1-43cca7a9ee37)
)

**5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!**

Untuk menambahkan kolom setelah kolom lain yaitu dengan perintah `AFTER`

![alt text](![Screenshot 2024-04-23 184212](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/f534486b-d243-4663-8148-6c7f023828a6)
)

**6. Ubah tipe data kolom id menjadi char(11)!**

Untuk mengubah type data yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] MODIFY nama_field tipe_data_baru(ukuran);`

![alt text](![Screenshot 2024-04-23 184230](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/688a398b-cbb0-4b14-92c2-d361f4a50c72)
)

**7. Ubah nama kolom phone menjadi hp (char 20)!**

Untuk mengubah kolom yaitu dengan perintah sebgai berikut :

`ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);`

![alt text](![Screenshot 2024-04-23 184240](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/e3a89468-4893-461e-9482-39f60c7fb308)
)

**8. Tambahkan kolom email setelah kolom hp**

![alt text](![Screenshot 2024-04-23 184250](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/e1c82759-4547-4940-a957-897c575efc93)
)

**9. Hapus kolom keterangan dari tabel!**

Untuk menghapus kolom dari tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] DROP nama_field;`

![alt text](![Screenshot 2024-04-23 184303](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/e29f576a-b9c3-400c-b6e1-d0b90950187c)
)

**10. Ganti nama tabel menjadi data_mahasiswa!**

Untuk mengganti nama tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] RENAME [nama_tabel_baru];`

![alt text](![Screenshot 2024-04-23 184314](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/b8508c05-f07f-47d7-a918-a48c4119c69b)
)

**11. Ganti nama field id menjadi nim!**

![alt text](![Screenshot 2024-04-23 184325](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/cc914cd3-cc19-4183-a1c9-39abb466f679)
)

**12. Jadikan nim sebagai PRIMARY KEY!**

Untuk menambahkan index atau key, gunakan perintah sebagai berikut :

tipe index :

- PRIMARY KEY
- UNIQUE KEY
- FULLTEXT

`ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);`

![alt text]![Screenshot 2024-04-23 184336](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/93e136f8-b8a6-4248-b3d2-93255cd1ebad)
)

**13. Jadikan kolom email sebagai UNIQUE KEY!**

Perintah nya sama seperti diatas, hanya saja diganti menjadi `UNIQUE KEY`

![alt text](![Screenshot 2024-04-23 184347](https://github.com/nurulaisyah14/TugasPraktikum1/assets/148174512/5e84fea8-21a7-442b-a4b7-e99af1ddcf8e)
)

# Pengertian INT
## 2. Apa Maksud Dari INT(11) ?

- INT(11) Adalah Nama Tipe Datanya Yaitu `Integer` dan Memiliki Panjang 11 Karakter. Yang dimaksud **int(11)** artinya suatu data yang dipakai atau digunakan dengan tipe data **int** atau **integer** dengan length atau panjang **karakter 11**.

# Penjelasan Kolom DESC
## 3. Ketika Kita Melihat Struktur Tabel Dengan Perintah DESC , Ada Kolom Null yang Berisi Yes dan No. Apa Maksudnya ?

- Apabila **Null** berisi **no**, maka data tersebut nantinya akan dilakukan *pengisian atau penginputan*. Sedangkan apabila **Null** berisi **yes**, maka artinya data tersebut akan *dikosongkan atau tidak dilakukan penginputan*.

## Finish
