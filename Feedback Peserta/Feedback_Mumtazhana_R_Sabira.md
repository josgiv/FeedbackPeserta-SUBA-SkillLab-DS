# Feedback untuk Mumtazhana R Sabira

---

Selamat, Mumtazhana! Notebook kamu menunjukkan penguasaan teknis yang baik dalam membangun pipeline Data Science secara lengkap. Ini adalah salah satu notebook terbaik yang kami evaluasi.

---

## Kelebihan

Notebook kamu memiliki beberapa keunggulan teknis:

- **SMOTE untuk Imbalanced Data** — Kamu memahami bahwa data yang tidak seimbang dapat menyebabkan bias pada model. Penggunaan SMOTE dari library `imblearn` menunjukkan pemahaman yang baik tentang preprocessing.

- **GridSearchCV untuk Hyperparameter Tuning** — Pencarian hyperparameter optimal dilakukan secara sistematis. Ini adalah pendekatan yang tepat.

- **imblearn Pipeline** — Mengintegrasikan SMOTE ke dalam pipeline adalah pendekatan yang proper untuk mencegah data leakage antara training dan testing set.

- **StratifiedKFold Cross-Validation** — Memastikan setiap fold memiliki proporsi kelas yang seimbang, menghasilkan evaluasi yang lebih reliable.

- **RobustScaler** — Pilihan scaler yang tepat untuk data dengan outlier, karena menggunakan median dan IQR.

- **Data Cleaning Berkualitas** — Berhasil menemukan dan memperbaiki nilai 'twenty' menjadi 20, serta melakukan winsorizing untuk handling outlier dengan IQR method.

- **Visualisasi Interaktif** — Penggunaan Plotly untuk visualisasi membuat analisis lebih jelas.

---

## Area Pengembangan

Meskipun sudah baik, ada ruang untuk improvement:

- **Eksplorasi Algoritma Lain** — Model dengan akurasi 50% menunjukkan bahwa Decision Tree mungkin bukan algoritma yang paling optimal untuk dataset ini. Ke depannya, bisa mencoba Random Forest atau algoritma lain.

---

## Kesimpulan

Pipeline ML yang kamu bangun sudah lengkap dan memenuhi kriteria dengan teknik yang tepat. Pertahankan standar kerja ini.

---

_Terima kasih atas dedikasi dalam menyelesaikan tugas ini._
