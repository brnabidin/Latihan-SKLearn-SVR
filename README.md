# Latihan-SKLearn-SVR

**Tahapan Latihan**

Tahapan pada latihan kali ini adalah sebagai berikut:

- Ubah data menjadi Dataframe.

- Pisahkan atribut dan label.

- Latih model SVR.

- Buat plot dari model.


# Codelab

Dataset yang akan kita gunakan adalah data tentang lama kerja seseorang dan gajinya. Dataset ini dapat diunduh pada tautan https://www.kaggle.com/karthickveerakumar/salary-data-simple-linear-regression berikut.

Setelah mengunggah dataset yang sudah di-unzip pada Google Colaboratory, pada cell pertama notebook kita impor library dasar yang dibutuhkan. Jangan lupa untuk mengubah berkas csv dari dataset menjadi dataframe Pandas.

![1](https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/7b5cfcdb-1b76-469b-b339-91ae289c88e2)

Selanjutnya kita bisa melihat apakah terdapat missing value pada dataset dengan fungsi .info(). Keluaran dari cell di bawah menunjukkan bahwa tidak ada missing value pada dataset.

![2](https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/df18083d-f137-49a8-b581-583cb6523a02)

<img width="325" alt="202004302219212b31ccb844f5b74fe020892558a3f2c4" src="https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/f654b1c4-8b3a-4325-aeeb-9e189bffad60">

Selanjutnya kita tampilkan 5 baris pertama dari dataframe.

![3](https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/2ee5dc5e-1ae3-4aeb-86de-abff401b77ae)

<img width="397" alt="20200430221937f8fcdbb22b2fd644fae316e777caf6bd" src="https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/e86704b9-3e0b-4368-9340-d9f2aad47753">

Kemudian kita pisahkan antara atribut dan label yang ingin diprediksi. Ketika hanya terdapat satu atribut pada dataframe, maka atribut tersebut perlu diubah bentuknya agar bisa diterima oleh model dari library SKLearn. Untuk mengubah bentuk atribut kita membutuhkan library numpy.

![4](https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/0ad574d9-2463-4857-88c3-aedfb63cb25d)

Berikutnya kita buat objek support vector regression dan di sini kita akan mencoba menggunakan parameter C = 1000, gamma = 0.05, dan kernel ‘rbf’. Setelah model dibuat kita akan melatih model dengan fungsi fit pada data.

![5](https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/9c44100a-3f34-4498-8b34-9849312d0f4c)

Terakhir kita bisa memvisualisasikan bagaimana model SVR kita menyesuaikan terhadap pola yang terdapat pada data menggunakan library matplotlib.

![6](https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/72d0c6e4-4854-4fb6-82fc-56d83a0178fb)

![2020043022261508ebe6b37a230570811447be760a3382](https://github.com/brnabidin/Latihan-SKLearn-SVR/assets/67081096/a5372abf-aa2f-48d7-8c0c-e34128d01f33)

Hasil visualisasi menunjukkan bahwa model yang kita kembangkan, belum mampu menyesuaikan terhadap pola pada data dengan baik. 
