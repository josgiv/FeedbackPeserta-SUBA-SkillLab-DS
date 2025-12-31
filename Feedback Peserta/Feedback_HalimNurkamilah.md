# Feedback untuk Halim Nurkamilah

---

Halim, notebook kamu menunjukkan ada upaya untuk menyelesaikan pipeline Data Science. Namun, ada kesalahan teknis yang perlu diperbaiki.

---

## Kelebihan

Notebook kamu memiliki beberapa aspek positif:

- **Ada Upaya Modeling** — Pipeline sampai ke tahapan modeling dan evaluation.

- **ydata_profiling** — Penggunaan automated profiling untuk EDA menunjukkan kemampuan memanfaatkan tools yang tepat.

---

## Masalah Teknis yang Perlu Diperbaiki

Ada kesalahan teknis yang signifikan:

**Handling Nilai Negatif dengan `.str.replace('-', '')` adalah Salah**

Ketika kamu menggunakan `.str.replace('-', '')` untuk menghilangkan tanda minus:

- Nilai `-5.00` menjadi `5.00`
- Ini salah secara matematis dan membuat data tidak representatif
- Nilai negatif memiliki makna berbeda dari nilai positif

Contoh dampak: Jika ada nilai `-5` (berarti minus 5), mengubahnya menjadi `5` berarti kamu membalikkan makna data sebesar 10 unit.

---

## Cara yang Benar

Untuk handling nilai negatif:

1. **Investigasi Dulu** — Apakah nilai negatif ini error entry atau memang valid?
2. **Jika Error** — Bisa diubah ke NaN atau median imputation
3. **Jika Valid** — Biarkan tetap negatif atau gunakan transformasi yang tepat
4. **Dokumentasikan Reasoning** — Jelaskan mengapa kamu memilih pendekatan tertentu

---

## Kesimpulan

Perbaiki handling nilai negatif. Pendekatan `str.replace('-', '')` adalah kesalahan teknis yang signifikan. Data yang dimodifikasi dengan cara ini tidak reliable untuk modeling.

---

_Pahami implikasi dari setiap transformasi data._
