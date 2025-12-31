# Feedback untuk Salwa Akmariza

---

Salwa, notebook kamu mengalami error fundamental yang mencegah eksekusi.

---

## Masalah Utama

**FileNotFoundError di Cell Pertama**

Notebook tidak dapat berjalan karena file data tidak ditemukan. Ini berarti:

- Tidak ada output yang bisa dievaluasi
- Pipeline sepenuhnya tidak berjalan
- Tidak memenuhi kriteria tugas

---

## Aspek Positif

Meskipun pipeline tidak berjalan, terlihat ada upaya yang baik:

- **Ada Kode Preprocessing** — Terlihat ada struktur kode untuk data cleaning dan preprocessing.

- **Niat untuk Analisis** — Struktur notebook menunjukkan pemahaman tentang workflow yang harus dilakukan.

---

## Langkah Perbaikan

Untuk memperbaiki notebook:

1. **Pastikan File Data Ada** — Upload file dataset ke environment yang sama dengan notebook.

2. **Cek Path File** — Pastikan path yang digunakan di `pd.read_csv()` sesuai dengan lokasi file.

3. **Test di Cell Pertama** — Sebelum submit, selalu pastikan cell pertama (data loading) berjalan tanpa error.

4. **Re-run All Cells** — Setelah perbaikan, restart kernel dan run all cells untuk memastikan semua berjalan.

Contoh path yang benar:

```python
# Jika file di folder yang sama
df = pd.read_csv('data.csv')

# Jika file di subfolder
df = pd.read_csv('./data/data.csv')

# Gunakan path relatif, bukan absolute
```

---

## Kesimpulan

Upload file data terlebih dahulu sebelum submit. Notebook yang tidak bisa di-run sama sekali tidak dapat dievaluasi karena tidak ada output yang bisa dinilai.

---

_Selalu test notebook sebelum submit. Pastikan semua cells berjalan._
