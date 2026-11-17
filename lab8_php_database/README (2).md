# Laporan Praktikum Lab 8 - Pemrograman Web OBE
**Mata Kuliah:** Pemrograman Web  
**Nama:** Tegar Addinia Putra  
**NIM:** 312510031  

---

## Tujuan Praktikum
1. Mahasiswa mampu memahami konsep dasar Database.
2. Mahasiswa mampu memahami konsep dasar CRUD (Create, Read, Update, Delete) menggunakan PHP.
3. Mahasiswa mampu membuat program CRUD sederhana menggunakan PHP dan MySQL.

---

## Langkah-Langkah Praktikum & Penjelasan

### 1. Persiapan dan Menjalankan MySQL Server
* Membuka aplikasi **XAMPP Control Panel**, lalu melakukan `Start` pada modul **Apache** dan **MySQL**.
* Memastikan status berubah menjadi hijau (running).
* Mengakses database melalui browser pada URL: `http://localhost/phpmyadmin/`

![XAMPP Control Panel](gambar/fig_8.1.png)

---

### 2. Membuat Database dan Tabel (`Studi Kasus Data Barang`)
* Membuat database baru dengan nama `latihan1`.
* Membuat tabel `data_barang` dengan struktur field sebagai berikut:
  * `id_barang`: INT (10), Primary Key, Auto Increment
  * `kategori`: VARCHAR (30)
  * `nama`: VARCHAR (30)
  * `gambar`: VARCHAR (100)
  * `harga_beli`: DECIMAL (10,0)
  * `harga_jual`: DECIMAL (10,0)
  * `stok`: INT (4)

```sql
CREATE DATABASE latihan1;

CREATE TABLE data_barang (
    id_barang int(10) auto_increment Primary Key,
    kategori varchar(30),
    nama varchar(30),
    gambar varchar(100),
    harga_beli decimal(10,0),
    harga_jual decimal(10,0),
    stok int(4)
);