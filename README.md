# TF-2-CNN-Fashion-MNIST

Langkah - langkah penggunaan dan keterangan:

1. Import library tensorflow dan muat data publik mnist serta bagi menjadi data train dan data test
2. Konvert dimensi data
3. Tentukan Jumlah Kelas
4. Membuat model CNN menggunakan functional API

- Convolution

convolution pada CNN yaitu sebuah operasi matematika pada dua buah fungsi yang kemudian menghasilkan fungsi ketiga. Fungsi ini menggabungkan 2 buah himpunan informasi dan menunjukkan bagaimana bentuk satu fungsi dimodifikasi oleh fungsi lainnya. CNN menggunakan convolution sebagai pengganti perkalian matriks umum

- Stride 

Stride adalah parameter yang menentukan berapa jumlah pergeseran filter. Jika nilai stride adalah 1, maka conv. filter akan bergeser sebanyak 1 pixels secara horizontal lalu vertical.

- ReLu

Aktivasi ReLU (Rectified Linear Unit) merupakan lapisan aktivasi pada model CNN yang mengaplikasikan fungsi f(x)=max(0,x) yang berarti fungsi ini melakukan thresholding dengan nilai nol terhadap nilai piksel pada input citra. Aktivasi ini membuat seluruh nilai piksel yang bernilai kurang dari nol pada suatu citra akan dijadikan 0.

![image](https://user-images.githubusercontent.com/87703066/180634000-d5289916-fbe4-4cf7-9557-521c99cc9f07.png)

- Flatten

Tahapan flattening adalah merubah dari matriks yang ada di pooling layer menjadi satu kolom saja (sebuah vektor tunggal). Nantinya vektor ini akan menjadi bagian dari input layer di artificial neural networks (ANN). Ilustrasinya sebagai berikut:

![image](https://user-images.githubusercontent.com/87703066/180634043-aed759af-243f-4286-acd7-9998143c5c6a.png)


- Dropout

Fungsi dari dropout adalah teknik untuk mencegah masalah overfitting Dropout ini direpresentasikan pada fully connected layer dengan cara kerja menonaktifkan beberapa neuron secara rendom yang tidak diperlukan

- Softmax 

Softmax menghitung probabilitas dari setiap kelas target atas semua kelas target yang memungkinkan dan akan membantu untuk menentukan kelas target untuk input yang diberikan. Keuntungan utama menggunakan Softmax adalah rentang probabilitas output dengan nilai 0 hingga 1, dan jumlah semua probabilitas akan sama dengan satu. Jika fungsi softmax digunakan untuk model multi-klasifikasi, dia akan mengembalikan peluang dari masing-masing kelas dan kelas target akan memiliki probabilitas tinggi.

![image](https://user-images.githubusercontent.com/87703066/180634301-1b84b578-469c-4fb7-9f60-748b6dd46c11.png)


- Adam

Adam adalah algoritma optimasi pengganti untuk stochastic gradient descent untuk training model deep learning. Adam menggabungkan sifat-sifat terbaik dari algoritma AdaGrad dan RMSProp untuk memberikan optimization algorithm yang dapat menangani sparse gradients pada noisy problem. (https://lms.onnocenter.or.id)

![image](https://user-images.githubusercontent.com/87703066/180634194-b9e673ce-bf99-49d1-a6bb-3561b5e97be3.png)

- Sparse Categorical Crossentropy

Fungsi loss ini memiliki tugas untuk mencari nilai gradien atau nilai yang menunjukan seberapa cepat nilai suatu variable berubah. Nilai tersebut nantinya akan digunakan untuk memperbarui nilai bobot. Categorical Cross-entropy (CC), meruapakan salah satu loss function yang biasa digunakan dalam klasifikasi yang memiliki kategori multi-class. Sedangkan untuk Sparse Categorical Cross-entropy (SCC) memiliki fungsi yang sama seperti Categorical Cross-entropy, hanya saja pada fungsi SCC data yang digunakan tidak dilakukan Hot-Encoding terlebih dahulu

5. Visualisasi Loss dan Akurasi

![image](https://user-images.githubusercontent.com/87703066/180634221-cd268c9e-fdec-4220-8483-fe8851c52013.png)
 ![image](https://user-images.githubusercontent.com/87703066/180634226-84fdd141-4588-4dae-983c-f1dc120d19d1.png)

6. Visualisasi Confusion Matrix

![image](https://user-images.githubusercontent.com/87703066/180634241-e432cc00-5bd6-4bb9-addc-0941eea63cd9.png)

7. Menampilkan contoh beberapa misklasifikasi
