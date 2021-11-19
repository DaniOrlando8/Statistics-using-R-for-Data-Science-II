Hubungan Pendapatan dengan Total Belanja dengan cor.test

Setelah melihat hubungan variabel pendapatan dengan total belanja menggunakan scatter plot diatas maka kita akan 
mengujinya, apakah benar-benar pendapatan memiliki pengaruh positif terhadap total belanja

Untuk melakukan uji korelasi pada R menggunakan perintah :

cor.test(data_intro$Pendapatan,data_intro$Total)

Berikut penjelasan function diatas :

Function cor.test digunakan untuk melihat hubungan secara statistik.
Pada korelasi test untuk mengujinya kita memakai t-test. Dengan hipotesis sebagai berikut:
Ho : tidak ada hubungan antara pendapatan dan total belanja.
Ha : terdapat hubungan antara pendapatan dan total belanja

Tugas Praktek

Lengkapi bagian [...1...] pada code editor untuk seperti yang ada pada bagian Lesson.

Jika berhasil maka keluaran akan sebagai berikut.

> cor.test(data_intro$Pendapatan,data_intro$Total)

	Pearson's product-moment correlation

data:  data_intro$Pendapatan and data_intro$Total
t = 3.1168, df = 18, p-value = 0.005957
alternative hypothesis: true correlation is not equal to 0
95 percent confidence interval:
 0.2026033 0.8197871
sample estimates:
      cor 
0.5920437 