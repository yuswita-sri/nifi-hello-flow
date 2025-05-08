# Catatan Latihan - NiFi Hello Flow

## Langkah-Langkah:

1. **Start NiFi**

   - Jalankan `run-nifi.bat` dari direktori `bin`.

2. **Akses UI**

   - Buka browser dan pergi ke `https://localhost:8443`
   - Login dengan username & password default dari `conf/initial-admin-identity` (jika ada).

3. **Buat Flow**

   - Tambahkan processor `GenerateFlowFile`.
   - Tambahkan processor `PutFile`.
   - Hubungkan keduanya via relationship `success`.
   - Atur `PutFile` dengan direktori output yang kamu inginkan.

4. **Jalankan Flow**

   - Klik tombol start di masing-masing processor.
   - File akan muncul di folder output.

5. **Hentikan dan Hapus**
   - Stop processor terlebih dahulu sebelum menghapus connection/processor.

## Catatan Teknis

- Jangan lupa mengatur permission folder output agar bisa ditulis oleh NiFi.
- Jika port 8080 bentrok, gunakan port lain seperti 8443.
