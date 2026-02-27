# ASSIGNMENT-1: TF-IDF & Text Preprocessing

Repositori ini berisi implementasi ekstraksi ciri teks menggunakan metode **TF-IDF (Term Frequency - Inverse Document Frequency)** yang dibangun sepenuhnya dari nol menggunakan bahasa Python, tanpa menggunakan library Machine Learning atau NLP eksternal seperti scikit-learn atau NLTK, sesuai dengan instruksi dosen pada tugas di e-lok.

Proyek ini disusun sebagai pemenuhan tugas mata kuliah Pengenalan Pola, Program Studi Ilmu Komputer, Universitas Gadjah Mada (UGM), atas nama:

**Nama    : Pison Golda Mountera**

**NIM     : 24/543770/PA/23107**

## Fitur Utama
Meskipun dibangun tanpa library pemrosesan teks, program ini dilengkapi dengan beberapa fitur:
1. **Text Preprocessing**:

    Meliputi *Case Folding*, *Punctuation Removal*, dan *Stopwords Filtering*.

2. **N-Gram Support**:
    
    Mendukung ekstraksi *unigram* maupun *n-gram* (misal: *bigram*).

3. **OOP Architecture**:

    Inti pemrosesan dibungkus dalam bentuk Class (Object-Oriented Programming) yang *reusable*, modular, dan siap diimplementasikan seperti API di sisi *Backend*.

4. **Search Engine Mini**:

    Mampu melakukan pencarian dokumen berdasarkan *query* menggunakan algoritma **Cosine Similarity**.

5. **OOV (Out of Vocabulary) Handling**:

    Sistem aman dari *error* apabila menerima kata kunci pencarian yang belum pernah ada di dalam *corpus* dokumen.

6. **Dynamic Data Loading**:

    Mengunduh dataset teks secara otomatis dari sumber eksternal (GitHub Gist) untuk kemudahan *running* kode.

## Prasyarat & Penggunaan
Logika inti perhitungan berjalan 100% menggunakan *native functions* Python. Satu-satunya *library* eksternal yang digunakan adalah **Pandas**, yang difungsikan murni dan eksklusif hanya untuk memformat matriks hasil akhir menjadi tabel *DataFrame* agar visualisasi data lebih elegan saat dibaca.

### Cara Menjalankan Kode
File utama berada dalam format Jupyter Notebook (.ipynb). Dapat dijalankan langsung melalui Google Colab dengan langkah berikut:
1. Buka file .ipynb
2. Klik tombol **"Open in Colab"** atau unduh dan *upload* ke Google Colab.
3. Klik **Run All**.

## Alur Logika / Pipeline
1. **Data Ingestion**:

    Membaca dokumen teks baris per baris.

2. **Preprocessing**:

    Membersihkan teks dan mengubahnya menjadi *tokens*.

3. **Vocabulary Building**:

    Membuat kamus kata unik dari seluruh korpus.

4. **TF Calculation**:

    Menghitung normalisasi frekuensi kata per dokumen.

5. **IDF Calculation**:

    Menghitung logaritma kelangkaan kata di seluruh korpus dokumen.

6. **TF-IDF Matrix**:

    Menghasilkan representasi vektor untuk setiap dokumen.

7. **Query Searching**:

    Menghitung skor kemiripan (Cosine Similarity) antara vektor *query* dengan vektor dokumen.

---
*Dibuat oleh Pison Golda Mountera | KOMA | Ilmu Komputer UGM*