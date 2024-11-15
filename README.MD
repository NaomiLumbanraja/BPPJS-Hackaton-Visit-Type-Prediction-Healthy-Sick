# Business Understanding
Tujuan utama dari analisis data ini adalah untuk membantu BPJS Kesehatan dalam meningkatkan efisiensi dan efektivitas pelayanan kesehatan melalui prediksi jenis kunjungan peserta di fasilitas kesehatan tingkat pertama (FKTP). 
Dengan prediksi yang tepat, BPJS Kesehatan dapat mengidentifikasi apakah kunjungan peserta bersifat preventif (sehat) atau untuk penanganan penyakit (sakit). 
Informasi ini memungkinkan BPJS dan FKTP untuk merencanakan sumber daya yang lebih optimal dan mengalokasikan tenaga medis, obat-obatan, serta peralatan sesuai kebutuhan nyata di lapangan.

Segmentasi peserta ini diharapkan dapat memberikan manfaat bisnis yang signifikan, termasuk:
1.	Mmengurangi potensi kelebihan atau kekurangan sumber daya dengan mengetahui jenis kunjungan yang akan datang, BPJS dan FKTP dapat menyiapkan tenaga medis, ruangan, dan peralatan yang sesuai untuk memenuhi kebutuhan peserta.
2.	Prediksi jenis kunjungan membantu FKTP memberikan pelayanan yang lebih cepat dan tepat. Kunjungan sehat mungkin membutuhkan pendekatan preventif, sedangkan kunjungan untuk penanganan penyakit membutuhkan pelayanan lebih intensif.
3.	Dengan mengetahui kebutuhan secara akurat, BPJS dapat mengalokasikan anggaran yang lebih efektif, misalnya dengan mengurangi pengeluaran untuk fasilitas preventif saat terjadi peningkatan kunjungan sakit, atau sebaliknya.
Hasil dari prediksi jenis kunjungan akan memberikan data yang berharga untuk evaluasi dan pengambilan keputusan yang lebih strategis di masa mendatang, misalnya dalam hal kampanye kesehatan preventif atau peningkatan layanan untuk penyakit tertentu.

**Data Understanding**
Data Understanding membantu dalam mengidentifikasi karakteristik, pola, dan kualitas data yang akan diolah. Tanpa pemahaman yang baik, proses data mining bisa menghasilkan interpretasi yang salah dan keputusan yang tidak tepat. Ada beberapa hal yang akan dilakukan pada tahapan ini:
1.	Pengumpulan Data: Mengumpulkan data yang diperlukan untuk analisis, termasuk informasi tentang diagnosis (ICD-10), jenis fasilitas kesehatan, pola rujukan, riwayat kunjungan, dan variabel-variabel lainnya yang relevan.
2.	Analisis Data: Melakukan eksplorasi awal untuk memahami distribusi data, pola umum, serta variabilitas pada fitur diagnosis, jenis fasilitas, pola rujukan, dan riwayat kunjungan.
3.	Validasi Data: Memastikan data yang dikumpulkan valid dan berkualitas, misalnya dengan memeriksa data yang hilang, mengidentifikasi nilai outlier, atau inkonsistensi dalam fitur.

**Data Prepraration**
1.	Memilah Data: Memilih fitur-fitur yang relevan untuk analisis prediksi, yaitu diagnosis (ICD-10), jenis fasilitas kesehatan, pola rujukan, dan riwayat kunjungan.
2.	Membersihkan Data: Menghapus data yang duplikat, mengisi data yang hilang, dan mengatasi nilai outlier untuk memastikan kualitas data tetap terjaga.
3.	Mengkonstruksi Data: Jika diperlukan, menciptakan fitur-fitur baru yang mungkin memiliki nilai prediktif lebih tinggi, seperti lama kunjungan rata-rata atau jumlah rujukan dalam periode tertentu.
4.	Menentukan Label Data: Menetapkan label target untuk klasifikasi, yaitu kategori "Sehat" atau "Sakit" berdasarkan data riwayat kunjungan atau deskripsi diagnosis.
5.	Mengintegrasikan Data: Menggabungkan data dari berbagai sumber jika diperlukan agar data yang digunakan lebih lengkap dan komprehensif.

**Modeling** 
1.	Membangun Skenario Pengujian: Menyusun skenario uji untuk menilai performa model, misalnya menggunakan data uji dan metrik evaluasi seperti akurasi, precision, recall, dan F1 score.
2.	Membangun Model: Menerapkan algoritma klasifikasi yang dipilih (SVM, KNN, atau Gradient Boosting) dan melatih model menggunakan data latih yang sudah disiapkan.

**Model Evaluation**
1.	Mengevaluasi Hasil Pemodelan: Mengevaluasi performa model dengan metrik yang relevan untuk memastikan model mampu memprediksi kunjungan sehat atau sakit dengan akurasi yang tinggi.
2.	Melakukan Review Proses Pemodelan: Meninjau ulang proses pemodelan untuk mencari kemungkinan peningkatan performa, misalnya dengan tuning hyperparameter atau mencoba algoritma lain.

**Deployment** 
1.	Membuat Rencana Deployment Model: Menyusun rencana untuk mengimplementasikan model ke dalam sistem produksi BPJS Kesehatan atau sistem informasi rumah sakit.
2.	Melakukan Deployment Model: Memasang model ke lingkungan produksi sehingga bisa digunakan untuk memprediksi jenis kunjungan secara otomatis pada data baru.
3.	Melakukan Rencana Pemeliharaan: Merencanakan pemeliharaan model, misalnya dengan pembaruan data secara berkala atau pemantauan performa model
4.	Melakukan Pemeliharaan: Menjalankan pemeliharaan rutin pada model untuk memastikan akurasi dan performa tetap optimal.

**Evaluation** 
1.	Melakukan Review Proyek: Melakukan evaluasi akhir atas hasil implementasi model, termasuk dampak bisnis yang dicapai (misalnya penghematan biaya atau peningkatan kualitas layanan).
2.	Membuat Laporan Akhir Proyek Menyusun laporan akhir yang mencakup hasil prediksi, analisis performa model, dan rekomendasi untuk langkah selanjutnya.

Dalam proyek ini, algoritma Support Vector Machine (SVM), K-Nearest Neighbor (KNN), atau Gradient Boosting akan digunakan untuk membangun model klasifikasi jenis kunjungan berdasarkan fitur-fitur seperti diagnosis (ICD-10), 
jenis fasilitas kesehatan, pola rujukan, dan riwayat kunjungan. Model ini diharapkan mampu memprediksi jenis kunjungan dengan akurasi tinggi, sehingga BPJS Kesehatan dan FKTP dapat melakukan perencanaan pelayanan kesehatan yang lebih tepat sasaran.

