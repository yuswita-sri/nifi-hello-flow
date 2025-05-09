# Catatan Flow Hari 2

## Alur Processor:

1. `GenerateFlowFile` → menghasilkan konten random
2. `UpdateAttribute` → menambahkan attribute baru seperti `filename`
3. `PutFile` → menyimpan hasil ke folder output

## Kendala:

- Tidak bisa hapus connection karena processor belum di-stop
- Tidak bisa delete karena masih ada aliran data

## Solusi:

- Stop processor sebelum menghapus
- Periksa relationship dan aktifkan auto-terminate jika tidak tersambung

## Pembelajaran:

- Pentingnya mengatur hubungan processor dengan benar
- NiFi fleksibel untuk dataflow sederhana dan kompleks
