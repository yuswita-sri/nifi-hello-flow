# NiFi Hello Flow

Proyek ini adalah latihan sederhana menggunakan Apache NiFi untuk memahami dasar-dasar alur data (data flow). Flow ini menghasilkan file teks dan menyimpannya ke folder output menggunakan dua processor: `GenerateFlowFile` dan `PutFile`.

## Tujuan

- Memahami cara kerja processor di NiFi.
- Mempelajari cara menghubungkan processor menggunakan relationship.
- Melakukan alur end-to-end dari pembuatan data hingga penyimpanan ke file.

## Tools

- Apache NiFi 1.28.1
- Java 16
- Sistem Operasi: Windows

## Struktur

- `GenerateFlowFile`: Membuat data dummy.
- `PutFile`: Menyimpan data ke direktori output.

## Output

File .txt sebanyak ~130 dokumen tersimpan di folder `nifi-output`.

## Lisensi

Proyek ini bersifat pembelajaran, bebas digunakan kembali untuk edukasi.
