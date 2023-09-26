# ProjectCapstoneMSIB5-HCAI
## Infinite Learning
Red Hat Certified System Administrator - IBM AI & Cybersecurity
Nama : Nur Romadhoni Hidayat
Asal : Pasuruan
Asal Kampus : Universitas Yudharta Pasuruan
Jurusan : Teknik Informatika

## Keterangan Projek
### Dataset Produksi Padi
Dataset ini diambil dari website kaggle : https://www.kaggle.com/datasets/ardikasatria/datasettanamanpadisumatera?resource=download 

![image](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/aa31ba50-32ef-4ed0-8fbe-7569990d4e63)

### Flow
![architecture](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/7b5425a2-2baa-4b40-b5fa-35fe71b538c8)
1. User mengirimkan dataset untuk percobaan AutoAI menggunakan pengaturan default dari sistem.
2. Beberapa model pipeline dihasilkan. Model pipeline pilihan dari papan peringkat disimpan sebagai buku catatan Jupyter.
3. Notebook Jupyter dijalankan dan model pipeline yang dimodifikasi dibuat di dalam notebook.
4. Model pipeline digunakan di Watson Machine Learning menggunakan API WML.

### Komponen
* IBM Watson Studio
![image](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/4da08a80-cacb-4b3c-a6fa-eb0407b152e0)
* IBM Watson Machine Learning
![image](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/15f13b41-fd25-4e16-a157-62187e3d826c)

### Hasil
![image](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/89a8b848-5e5f-4bd3-b8b4-9b6af8e1c368)
Hasil dari tiap pipeline
![image](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/1c36a8d8-af26-4a60-83fc-7f1a8c5ccc6b)
Perbedaan tiap pipeline
![image](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/46e4531e-9d42-4d8e-9672-ef2ae7b3dfe0)
![image](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/55d87add-2f51-4e30-a9af-ab921cdfc8e5)
Feature summary
![image](https://github.com/TryAgain15/ProjectCapstoneMSIB5/assets/118412595/5097cf6e-e253-4d7e-af90-df6afc92dcdc)

## Kesimpulan
Berdasarkan dari hasil model tersebut, dapat disimpulkan bahwa : 
1. Algoritma yang digunakan adalah LGBM karena sangat cocok untuk hasil model ini karena ia efisien dan cepat dalam menangani data berukuran besar, mendukung beragam fitur, dan memiliki kemampuan yang kuat dalam menjelaskan variasi dalam data, seperti yang ditunjukkan oleh nilai R-squared yang tinggi pada hasil model.

2. Kualitas Model: Model yang digunakan ini memiliki tingkat akurasi yang cukup baik dalam memprediksi produksi padi berdasarkan fitur-fitur yang digunakan. Hal ini ditunjukkan oleh nilai R-squared yang tinggi pada Holdout Score (0.989), yang menunjukkan bahwa model memiliki kemampuan yang sangat baik dalam menjelaskan variasi dalam data validasi.

3. Overfitting: Terdapat perbedaan yang cukup besar antara RMSE pada data pelatihan (Cross Validation Score) dan RMSE pada data validasi (Holdout Score), yang menunjukkan bahwa model mungkin mengalami overfitting pada data pelatihan. Hal ini perlu dipertimbangkan untuk memastikan bahwa model dapat menggeneralisasi dengan baik ke data yang belum pernah dilihat sebelumnya.

4. Tingkat Akurasi: Meskipun tingkat akurasi model pada data pelatihan cukup tinggi (R-squared 0.942), perlu diingat bahwa data pelatihan mungkin tidak mencakup semua variasi yang mungkin terjadi di lapangan. Oleh karena itu, penting untuk melakukan validasi model secara berkala menggunakan data aktual produksi.

5. Prediksi Produksi: Hasil prediksi produksi padi yang diberikan oleh model dapat digunakan sebagai panduan awal dalam perencanaan pertanian. Namun, perbandingan dengan data aktual produksi yang diperbarui secara berkala sangat penting untuk menilai akurasi model.

6. Konteks Lokal: Selain faktor-faktor dalam model, praktik pertanian lokal, varietas tanaman, dan kondisi tanah juga perlu dipertimbangkan dalam pengambilan keputusan pertanian yang lebih rinci.

Kesimpulannya, hasil model Anda adalah alat yang berguna untuk memberikan perkiraan produksi padi berdasarkan data yang ada. Namun, untuk pengambilan keputusan pertanian yang lebih tepat, perlu dipertimbangkan faktor-faktor alam, praktik pertanian, dan pemantauan kondisi aktual lapangan. Selalu perbarui model dan
