Hubungan Produk dengan Tingkat Kepuasan dengan chisq.test
Berdasarkan kasus diatas kita akan melihat hubungan antara data kategorik dan kategorik, yaitu variabel jenis 
produk dan tingkat kepuasan. Sebelum menguji hubungannya, sebaiknya dilakukan tabulasi silang sebagai analisis 
deskriptif. Selanjutnya analisis inferensia yaitu menguji apakah ada hubungan maka dapat digunakan chi-square test.

Untuk melakukan tabulasi dan uji statistik chi-square test pada R tahapannya sebagai berikut :

table(data_intro$Produk,data_intro$Tingkat.Kepuasan)
chisq.test(table(data_intro$Produk,data_intro$Tingkat.Kepuasan))

Perintah table untuk melihat tabulasi antar variabel kategorik, sedangkan perintah chisq.test digunakan untuk 
melihat hubungan secara statistik.

Dengan hipotesis sebagai berikut :

Ho : tidak ada hubungan antara jenis produk dan tingkat kepuasan.
Ha : terdapat hubungan antara jenis produk dan tingkat kepuasan  
 

Tugas Praktek

Gantilah bagian [...1...] dan [...2...] masing-masing untuk mencari tabulasi antar variabel kategorik dan 
melihat hubungan secara statistik dengan chi-square test.

> ## Carilah tabulasi silang antara kolom jenis produk (Produk) dan tingkat kepuasan (Tingkat.Kepuasan) dari variable data_intro
> table(data_intro$Produk,data_intro$Tingkat.Kepuasan)
   
    1 2 3
  A 0 1 3
  B 2 0 2
  C 1 2 1
  D 2 2 1
  E 2 0 1

> ## Analisis bagaimana hubungan jenis produk dengan tingkat kepuasan mengunakan uji korelasi
> chisq.test(table(data_intro$Produk,data_intro$Tingkat.Kepuasan))

	Pearson's Chi-squared test

data:  table(data_intro$Produk, data_intro$Tingkat.Kepuasan)
X-squared = 7.95, df = 8, p-value = 0.4384

