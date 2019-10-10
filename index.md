## Nama : Oktaviana Dwi Sujatmiko

## NIM : 180411100021

## TEKNIK INFORMATIKA

# PENAMBANGAN DATA 3B





# Statistik Deskriptif

Statistik deskriptif adalah salah satu bagian dari ilmu statistika yang berhubungan dengan aktivitas penghimpunan, penataan, peringkasan dan penyajian data dengan harapan agar data lebih bermakna, mudah dibaca dan mudah dipahami oleh pengguna data. Statistik deskriptif hanya sebatas memberikan deskripsi atau gambaran umum tentang karakteristik objek yang diteliti tanpa maksud untuk melakukan generalisasi sampel terhadap populasi.

​	Kegiatan dalam statistik deskriptif meliputi pengumpulan, pengelompokan dan pengolahan data yang selanjutnya akan menghasilkan ukuran-ukuran statistik seperti frekuensi, pemusatan data, penyebaran data, kecenderungan suatu gugus data dan lain-lain. Selain itu, agar data lebih mudah dibaca dan dipahami maka data dapat diringkas dalam bentuk tabulasi atau disajikan dalam bentuk grafik atau diagram, beberapa yang akan kita bahas yaitu :

- Rata-rata

- Median

- Modus

- Variansi

- Standar Deviasi

- Range 

- Quartil

- Skewness

  ## 1. Rata - rata

  ​	Rata-rata adalah nilai yang mewakili sekelompok data. Rata-rata diperoleh dari penjumlahan seluruh nilai data dibagi dengan banyaknya data.

  ## 2. Median

  ​	Untuk data miring (asimetris), ukuran pusat data yang lebih baik adalah median, yang merupakan nilai tengah dalam satu set nilai data yang diurutkan. Ini adalah nilai yang memisahkan separuh data yang lebih tinggi dari data tersebut dan sebagian data yang lebih rendah dari data tersebut. Dalam probabilitas dan statistik, median umumnya berlaku untuk data numerik; namun, kami dapat memperluas konsep menjadi data ordinal. Misalkan kumpulan N data yang diberikan untuk atribut X diurutkan dalam urutan naik. Jika N ganjil, maka median adalah nilai tengah dari data yang ordinal. Jika N adalah genap, maka mediannya tidak unik; dihitung dengan rata rata dari nilai 

## 3.  Modus

 Modus adalah nilai yang sering muncul dalam sekelompok data.



## 4. Variansi dan standart Variansi

*Varian* adalah rata-rata jarak kuadrat antara data ke rata-rata.



## 5. Range

*Jangkauan (Range)* adalah ukuran dari selisih nilai maksimum dengan nilai minimum yang ada dalam sekelompok data.R = x_{max} - x_{min} *R*=xmax−xmin



## 6. Quartil

Kuartil memberikan gambaran pusat distribus, penyebaran, dan bentuk distribusi. Kuartil satu, dilambangkan oleh Q1, adalah persentil ke-25. Nilai ini menunjukan 25% terendah dari data. Kuartil ketiga, dilambangkan oleh Q3, adalah persentil ke-75 - itu memisahkan data 75% dari terendah data (atau 25% dari tertinggi data. 

## 7. Skewness

​	Derajat distorsi dari kurva lonceng simetris atau distribusi normal. Ini mengukur kurangnya simetri dalam distribusi data Untuk menghitung derajat distorisi dapat menggunakan Koefisien Kemencengan Pearson yang diperoleh dengan menggunakan nilai selisih rata-rata dengan modus dibagi simpangan baku.

![](C:\Users\ASUS\newdatamining\foto\10.PNG)

![11](C:\Users\ASUS\newdatamining\foto\11.PNG)

![12](C:\Users\ASUS\newdatamining\foto\12.PNG)

![13](C:\Users\ASUS\newdatamining\foto\13.PNG)

# Mengukur Jarak Atribut Binary

#### Mengukur Jarak Tipe categorical

### *Overlay Metric*

Ketika semua atribut adalah bertipe nominal, ukuran jarak yang paling sederhana adalah dengan Ovelay Metric (OM) yang dinyatakan dengan dimana nn adalah banyaknya atribut, ai(x)ai(x) dan ai(y)ai(y) adalah nilai atribut ke ii yaitu AiAi dari masing masing objek xx dan yy, δ (ai(x),ai(y))δ (ai(x),ai(y)) adalah 0 jika ai(x)=ai(y)ai(x)=ai(y) dan 1 jika sebaliknya.

OM banyak digunakan oleh instance-based learning dan locally weighted learning. Jelas sekali , ini sedikit beruk untuk mengukur jarak antara masing-masing pasangan sample, karena gagal memanfaatkan tambahan informasi yang diberikan oleh nilai atribut nominal yang bisa membantu dalam generalisasi.

### *Value Difference Metric (VDM)*

VDM dikenalkan oleh Standfill and Waltz, versi sederhana dari VDM tanpa skema pembobotan didefinsisikan dengan dimana CCadalah banyaknya kelas, P(c|ai(x))P(c|ai(x)) adalah probabilitas bersyarat dimana kelas xx adalah cc dari atribut AiAi, yang memiliki nilai ai(x)ai(x), P(c|ai(y))P(c|ai(y)) adalah probabilitas bersyarat dimana kelas yy adalah cc dengan atribut AiAi memiliki nilai ai(y)ai(y)

VDM mengasumsikan bahwa dua nilai dari atribut adalah lebih dekat jika memiliki klasifikasi sama. Pendekatan lain berbasi probabilitas adalah SFM (Short and Fukunaga Metric) yang kemudian dikembangkan oleh Myles dan Hand dan didefinisikan.

### *Minimum Risk Metric (MRM)*

Ukuran ini dipresentasikan oleh Blanzieri and Ricci, berbeda dari SFM yaitu meminimumkan selisih antara kesalahan berhingga dan kesalahan asymtotic. MRM meminimumkan risk of misclassification yang didefinisikan.

## Mengukur Jarak Tipe Ordinal

Nilai-nilai atribut ordinal memiliki urutan atau peringkat, namun besarnya antara nilai-nilai berturut-turut tidak diketahui. Contohnya tingkatan kecil, sedang, besar untuk atribut ukuran. Atribut ordinal juga dapat diperoleh dari diskritisasi atribut numerik dengan membuat rentang nilai ke dalam sejumlah kategori tertentu. Kategori-kategori ini disusun dalam peringkat. Yaitu, rentang atribut numerik dapat dipetakan ke atribut ordinal ff yang memiliki MfMf state. Misalnya, kisaran suhu atribut skala-skala (dalam Celcius)dapat diatur ke dalam status berikut: −30 hingga −10, −10 hingga 10, 10 hingga 30, masing-masing mewakili kategori suhu dingin, suhu sedang, dan suhu hangat. MM adalah jumlah keadaan yang dapat dilakukan oleh atribut ordinalmemiliki. State ini menentukan peringkat 1,...,Mf1,...,Mf

Perlakuan untuk atribut ordinal adalah cukup sama dengan atribut numerik ketika menghitung disimilarity antara objek. Misalkan ff adalah atribut-atribut dari atribut ordinal dari nn objek. Menghitung disimilarity terhadap f fitur sebagai berikut:

- Nilai ff untuk objek ke-ii adalah xifxif, dan ff memiliki MfMf status urutan , mewakili peringkat 1,..,Mf1,..,Mf Ganti setiap xifxif dengan peringkatnya, rif∈{1...Mf}rif∈{1...Mf}

- Karena setiap atribut ordinal dapat memiliki jumlah state yang berbeda, diperlukan untuk memetakan rentang setiap atribut ke [0,0, 1.0] sehingga setiap atribut memiliki bobot yang sama. Perl melakukan normalisasi data dengan mengganti peringkat rifrif denganzif=rif−1Mf−1zif=rif−1Mf−1

- Dissimilarity kemudian dihitung dengan menggunakan ukuran jarak seperti atribut numerik dengan data yang baru setelah ditransformasi $ z _ { i f }

  ## Menghitung Jarak Tipe Campuran

  Menghitung ketidaksamaan antara objek dengan atribut campuran yang berupa nominal, biner simetris, biner asimetris, numerik, atau ordinal yang ada pada kebanyakan databasae dapat dinyatakan dengan memproses semua tipe atribut secara bersamaan. Salah satu teknik tersebut menggabungkan atribut yang berbeda ke dalam matriks ketidaksamaan tunggal dan menyatakannya dengan skala interval antar [0,0,1.0][0,0,1.0]. Misalkan data berisi atribut pp tipe campuran. Ketidaksamaan (disimilarity ) antara objek ii dan jj dinyatakan dengan

  d(i,j)=∑pf=1δ(f)ijd(f)ij∑pf=1δ(f)ijd(i,j)=∑f=1pδij(f)dij(f)∑f=1pδij(f)

  dimana δfij=0δijf=0 - jika xifxif atau xjfxjf adalah hilang (i.e., tidak ada pengukuran dari atribut f untuk objek ii atau objek jj)

  - jika xif=xjf=0xif=xjf=0 dan
  - atribut ff adalah binary asymmetric,

  selain itu δfij=1δijf=1

  Kontribusi dari atribut ff untuk dissimilarity antara i dan j (yaitu.dfijdijf) dihitung bergantung pada tipenya,

  - Jika ff adalah numerik, dfij=∥xif−xjf∥maxhxhf−minhxhfdijf=‖xif−xjf‖maxhxhf−minhxhf, di mana h menjalankan semua nilai objek yang tidak hilang untuk atribut f

  - Jika ff adalah nominal atau binary,$d_{ij}^{f}=0 $jika xif=xjfxif=xjf, sebaliknya dfij=1dijf=1

  - Jika ff adalah ordinal maka hitung rangking rifrif dan zif=rif−1Mf−1zif=rif−1Mf−1 , dan perlakukan zifzif sebagai numerik.

    ![](C:\Users\ASUS\newdatamining\foto\14.PNG)
    
    ![15](C:\Users\ASUS\newdatamining\foto\15.PNG)
    
    ![16](C:\Users\ASUS\newdatamining\foto\16.PNG)

## SELECTION FEATURE

Pemilihan (seleksi) data dari sekumpulan data operasional perlu dilakukan sebelum tahap penggalian informasi dalam KDD dimulai. Data hasil seleksi yang digunakan untuk proses data mining, disimpan dalam suatu berkas, terpisah dari basis data operasional.



Entropy Target

- Entropy (S) merupakan jumlah bit yang diperkirakan dibutuhkan untuk dapat mengekstrak suatu kelas (+ atau -) dari sejumlah data acak pada ruang sampel S.

- Entropy dapat dikatakan sebagai kebutuhan bit untuk menyatakan suatu kelas.

- Entropy digunakan untuk mengukur ketidakaslian S.

  ![](C:\Users\ASUS\newdatamining\foto\8.PNG)

![](C:\Users\ASUS\newdatamining\foto\2.PNG)

![3](C:\Users\ASUS\newdatamining\foto\3.PNG)

![4](C:\Users\ASUS\newdatamining\foto\4.PNG)



Information GAIN

- Gain (S,A) merupakan perolehan informasi dari atribut A relative terhadap output data S.

- Perolehan informasi didapat dari output data atau variable dependent S yang dikelompokkan berdasarkan atribut A, dinotasikan dengan gain (S,A).

  ![](C:\Users\ASUS\newdatamining\foto\9.PNG)

![](C:\Users\ASUS\newdatamining\foto\5.PNG)

![6](C:\Users\ASUS\newdatamining\foto\6.PNG)

![7](C:\Users\ASUS\newdatamining\foto\7.PNG)

##    Naive Bayes 

**Algoritma Naive Bayes** merupakan sebuah metoda klasifikasi menggunakan metode probabilitas dan statistik yg dikemukakan oleh ilmuwan Inggris Thomas Bayes. **Algoritma Naive Bayes** memprediksi peluang di masa depan berdasarkan pengalaman di masa sebelumnya sehingga dikenal sebagai Teorema Bayes. Ciri utama dr Naïve Bayes Classifier ini adalah asumsi yg sangat kuat (naïf) akan independensi dari masing-masing kondisi / kejadian.

 

Naive Bayes Classifier bekerja sangat baik dibanding dengan model classifier lainnya. Hal ini dibuktikan pada jurnal *Xhemali, Daniela, Chris J. Hinde, and Roger G. Stone. “Naive Bayes vs. decision trees vs. neural networks in the classification of training web pages.” (2009),* mengatakan bahwa “Naïve Bayes Classifier memiliki tingkat akurasi yg lebih baik dibanding model classifier lainnya”.

 

Keuntungan penggunan adalah bahwa metoda ini hanya membutuhkan jumlah data pelatihan (training data) yang kecil untuk menentukan estimasi parameter yg diperlukan dalam proses pengklasifikasian. Karena yg diasumsikan sebagai variabel independent, maka hanya varians dari suatu variabel dalam sebuah kelas yang dibutuhkan untuk menentukan klasifikasi, bukan keseluruhan dari matriks kovarians.

 

Tahapan dari proses algoritma Naive Bayes adalah:

1. Menghitung jumlah kelas / label.
2. Menghitung Jumlah Kasus Per Kelas
3. Kalikan Semua Variable Kelas
4. Bandingkan Hasil Per Kelas

 

#### **1. Kelebihan & Kekurangan Naive Bayes**

**Kelebihan**

- Mudah untuk dibuat
- Hasil bagus

**Kekurangan**

- Asumsi independence antar atribut membuat akurasi berkurang (karena biasanya ada keterkaitan)

  ![](C:\Users\ASUS\newdatamining\foto1\51.PNG)

  

  **Keterangan :**
  ***x*** : Data dengan class yang belum diketahui
  ***c*** : Hipotesis data merupakan suatu class spesifik
  ***P(c|x)*** : Probabilitas hipotesis berdasar kondisi (posteriori probability)
  ***P(c)*** : Probabilitas hipotesis (prior probability)
  ***P(x|c)*** : Probabilitas berdasarkan kondisi pada hipotesis
  ***P(x)*** : Probabilitas c

   

  Rumus diatas menjelaskan bahwa peluang masuknya sampel karakteristik tertentu dalam kelas C (Posterior) adalah peluang munculnya kelas C (sebelum masuknya sampel tersebut, seringkali disebut prior), dikali dengan peluang kemunculan karakteristik karakteristik sampel pada kelas C (disebut juga likelihood), dibagi dengan peluang kemunculan karakteristik  sampel secara global ( disebut juga evidence). 

  Nilai Evidence selalu tetap untuk setiap kelas pada satu sampel. Nilai dari posterior tersebut nantinya akan dibandingkan dengan nilai nilai posterior kelas lainnya untuk menentukan ke kelas apa suatu sampel akan diklasifikasikan. Penjabaran lebih lanjut rumus Bayes tersebut dilakukan dengan menjabarkan *(c|x1,…,xn)* menggunakan aturan perkalian 

  

  Dapat dilihat bahwa hasil penjabaran tersebut menyebabkan semakin banyak dan semakin kompleksnya faktor faktor syarat yang mempengaruhi nilai probabilitas, yang hampir mustahil untuk dianalisa satu persatu. Akibatnya, perhitungan tersebut menjadi sulit untuk dilakukan. Disinilah digunakan asumsi independensi yang sangat tinggi (naif), bahwa masing masing petunjuk saling bebas (independen) satu sama lain. Dengan asumsi tersebut, maka berlaku suatu kesamaan sebagai berikut:

  ![](C:\Users\ASUS\newdatamining\foto1\52.PNG)

  

  Persamaan diatas merupakan model dari **Teorema Naive Bayes** yang selanjutnya akan digunakan dalam proses klasifikasi. Untuk klasifikasi dengan data kontinyu digunakan rumus Densitas Gauss :

  ![](C:\Users\ASUS\newdatamining\foto1\53.PNG)

###### pengambilan data set

```python
from sklearn import datasets`
`from pandas import *`
`from numpy import *`
`from math import *`

`from IPython.display import HTML, display; from tabulate import tabulate`
```





```python
def table(df): display(HTML(tabulate(df, tablefmt='html', headers='keys', showindex=False)))`

`from sklearn import datasets`
`from pandas import *`
`from numpy import *`
`from math import *`

`from IPython.display import HTML, display; from tabulate import tabulate`
`def table(df): display(HTML(tabulate(df, tablefmt='html', headers='keys', showindex=False)))
```



| sepal length (cm) | sepal width (cm) | petal length (cm) | petal width (cm) |   class    |
| ----------------: | ---------------: | ----------------: | ---------------: | :--------: |
|               4.4 |                3 |               1.3 |              0.2 |   setosa   |
|                 5 |              3.6 |               1.4 |              0.2 |   setosa   |
|               7.7 |              3.8 |               6.7 |              2.2 | virginica  |
|               7.2 |              3.2 |                 6 |              1.8 | virginica  |
|                 5 |              3.4 |               1.6 |              0.4 |   setosa   |
|               6.4 |              2.7 |               5.3 |              1.9 | virginica  |
|                 5 |              3.5 |               1.3 |              0.3 |   setosa   |
|               6.2 |              2.2 |               4.5 |              1.5 | versicolor |
|               6.3 |              2.8 |               5.1 |              1.5 | virginica  |
|               5.7 |              4.4 |               1.5 |              0.4 |   setosa   |
|               4.6 |              3.6 |                 1 |              0.2 |   setosa   |
|               7.4 |              2.8 |               6.1 |              1.9 | virginica  |
|               5.5 |              2.4 |               3.8 |              1.1 | versicolor |
|                 6 |              3.4 |               4.5 |              1.6 | versicolor |
|               4.9 |              3.1 |               1.5 |              0.2 |   setosa   |
|               4.5 |              2.3 |               1.3 |              0.3 |   setosa   |
|               7.3 |              2.9 |               6.3 |              1.8 | virginica  |
|               6.5 |                3 |               5.5 |              1.8 | virginica  |
|               5.5 |              2.4 |               3.7 |                1 | versicolor |
|               6.9 |              3.2 |               5.7 |              2.3 | virginica  |
|               7.2 |                3 |               5.8 |              1.6 | virginica  |
|               4.9 |                3 |               1.4 |              0.2 |   setosa   |
|               6.8 |              3.2 |               5.9 |              2.3 | virginica  |
|               5.6 |                3 |               4.5 |              1.5 | versicolor |
|                 5 |              2.3 |               3.3 |                1 | versicolor |
|               5.6 |              2.5 |               3.9 |              1.1 | versicolor |
|               6.3 |              2.9 |               5.6 |              1.8 | virginica  |
|               6.4 |              3.2 |               5.3 |              2.3 | virginica  |
|               4.9 |              2.4 |               3.3 |                1 | versicolor |
|               4.9 |              3.6 |               1.4 |              0.1 |   setosa   |

`test = [5,6,8,9]`
`print("sampel data: ", test)`

```
sampel data:  [5, 6, 8, 9]
```



###### identifikasi per grub class target untuk data mining serta perhitungan Probabilitas Prior dan Likehood



```python
dataset_classes = {}`
`for key,group in dataset.groupby('class'):`
    `mu_s = [group[c].mean() for c in group.columns[:-1]]`
    `sigma_s = [group[c].std() for c in group.columns[:-1]]`
    `dataset_classes[key] = [group, mu_s, sigma_s]`
    `print(key, "===>")`
    `print('Mu_s =>', array(mu_s))`
    `print('Sigma_s =>', array(sigma_s))`
    `table(group)`
`def numericalPriorProbability(v, mu, sigma):`
    `return (1.0/sqrt(2 * pi * (sigma ** 2))*exp(-((v-mu)**2)/(2*(sigma**2))))`

`def categoricalProbability(sample,universe):`
    `return sample.shape[0]/universe.shape[0]`

`Ps = ([[y]+[numericalPriorProbability(x, d[1][i], d[2][i]) for i,x in enumerate(test)]+`
          `[categoricalProbability(d[0],dataset)] for y,d in dataset_classes.items()])`

`table(DataFrame(Ps, columns=["classes"]+["P( %d | C )" % d for d in test]+["P( C )"]))`
`Pss = ([[r[0], prod(r[1:])] for r in Ps])`
`PDss = DataFrame(Pss, columns=['class', 'probability']).sort_values('probability')[::-1]`
`table(PDss)
```



```
setosa ===>
Mu_s => [4.89 3.35 1.37 0.25]
Sigma_s => [0.36040101 0.55025247 0.16363917 0.09718253]
```



| sepal length (cm) | sepal width (cm) | petal length (cm) | petal width (cm) |  class |
| ----------------: | ---------------: | ----------------: | ---------------: | -----: |
|               4.4 |                3 |               1.3 |              0.2 | setosa |
|                 5 |              3.6 |               1.4 |              0.2 | setosa |
|                 5 |              3.4 |               1.6 |              0.4 | setosa |
|                 5 |              3.5 |               1.3 |              0.3 | setosa |
|               5.7 |              4.4 |               1.5 |              0.4 | setosa |
|               4.6 |              3.6 |                 1 |              0.2 | setosa |
|               4.9 |              3.1 |               1.5 |              0.2 | setosa |
|               4.5 |              2.3 |               1.3 |              0.3 | setosa |
|               4.9 |                3 |               1.4 |              0.2 | setosa |
|               4.9 |              3.6 |               1.4 |              0.1 | setosa |



```
versicolor ===>
Mu_s => [5.5375 2.575  3.9375 1.225 ]
Sigma_s => [0.44057592 0.40970373 0.51252178 0.26049404]
```



| sepal length (cm) | sepal width (cm) | petal length (cm) | petal width (cm) |      class |
| ----------------: | ---------------: | ----------------: | ---------------: | ---------: |
|               6.2 |              2.2 |               4.5 |              1.5 | versicolor |
|               5.5 |              2.4 |               3.8 |              1.1 | versicolor |
|                 6 |              3.4 |               4.5 |              1.6 | versicolor |
|               5.5 |              2.4 |               3.7 |                1 | versicolor |
|               5.6 |                3 |               4.5 |              1.5 | versicolor |
|                 5 |              2.3 |               3.3 |                1 | versicolor |
|               5.6 |              2.5 |               3.9 |              1.1 | versicolor |
|               4.9 |              2.4 |               3.3 |                1 | versicolor |



```
virginica ===>
Mu_s => [6.86666667 3.05833333 5.775      1.93333333]
Sigma_s => [0.48679533 0.29374799 0.45949577 0.27743413]
```



| sepal length (cm) | sepal width (cm) | petal length (cm) | petal width (cm) |     class |
| ----------------: | ---------------: | ----------------: | ---------------: | --------: |
|               7.7 |              3.8 |               6.7 |              2.2 | virginica |
|               7.2 |              3.2 |                 6 |              1.8 | virginica |
|               6.4 |              2.7 |               5.3 |              1.9 | virginica |
|               6.3 |              2.8 |               5.1 |              1.5 | virginica |
|               7.4 |              2.8 |               6.1 |              1.9 | virginica |
|               7.3 |              2.9 |               6.3 |              1.8 | virginica |
|               6.5 |                3 |               5.5 |              1.8 | virginica |
|               6.9 |              3.2 |               5.7 |              2.3 | virginica |
|               7.2 |                3 |               5.8 |              1.6 | virginica |
|               6.8 |              3.2 |               5.9 |              2.3 | virginica |
|               6.3 |              2.9 |               5.6 |              1.8 | virginica |
|               6.4 |              3.2 |               5.3 |              2.3 | virginica |



|    classes | P( 5 \| C ) | P( 6 \| C ) | P( 8 \| C ) |  P( 9 \| C ) |   P( C ) |
| ---------: | ----------: | ----------: | ----------: | -----------: | -------: |
|     setosa |     1.05656 | 6.66694e-06 |           0 |            0 | 0.333333 |
| versicolor |     0.43022 | 6.50426e-16 | 1.77008e-14 | 5.48538e-194 | 0.266667 |
|  virginica | 0.000525523 | 2.27126e-22 | 7.03175e-06 | 1.87532e-141 |      0.4 |



|      class | probability  |
| ---------: | :----------: |
|  virginica | 6.29591e-172 |
| versicolor | 7.2453e-224  |
|     setosa |      0       |

###### Percobaan

```python
`def predict(sampel):`
    `priorLikehoods = ([[y]+[numericalPriorProbability(x, d[1][i], d[2][i]) for i,x in enumerate(sampel)]+`
          `[categoricalProbability(d[0],dataset)] for y,d in dataset_classes.items()])`
    `products = ([[r[0], prod(r[1:])] for r in priorLikehoods])`
    `result = DataFrame(products, columns=['class', 'probability']).sort_values('probability')[::-1]`
    `return result.values[0,0]`

`dataset_test = DataFrame([list(d)+[predict(d[:4])] for d in data], columns=list(dataset.columns)+['predicted class (by predict())'])`
`table(dataset_test)`
```



| sepal length (cm) | sepal width (cm) | petal length (cm) | petal width (cm) |      class | predicted class (by predict()) |
| ----------------: | ---------------: | ----------------: | ---------------: | ---------: | :----------------------------: |
|               5.1 |              3.5 |               1.4 |              0.2 |     setosa |             setosa             |
|               4.9 |                3 |               1.4 |              0.2 |     setosa |             setosa             |
|               4.7 |              3.2 |               1.3 |              0.2 |     setosa |             setosa             |
|               4.6 |              3.1 |               1.5 |              0.2 |     setosa |             setosa             |
|                 5 |              3.6 |               1.4 |              0.2 |     setosa |             setosa             |
|               5.4 |              3.9 |               1.7 |              0.4 |     setosa |             setosa             |
|               4.6 |              3.4 |               1.4 |              0.3 |     setosa |             setosa             |
|                 5 |              3.4 |               1.5 |              0.2 |     setosa |             setosa             |
|               4.4 |              2.9 |               1.4 |              0.2 |     setosa |             setosa             |
|               4.9 |              3.1 |               1.5 |              0.1 |     setosa |             setosa             |
|               5.4 |              3.7 |               1.5 |              0.2 |     setosa |             setosa             |
|               4.8 |              3.4 |               1.6 |              0.2 |     setosa |             setosa             |
|               4.8 |                3 |               1.4 |              0.1 |     setosa |             setosa             |
|               4.3 |                3 |               1.1 |              0.1 |     setosa |             setosa             |
|               5.8 |                4 |               1.2 |              0.2 |     setosa |             setosa             |
|               5.7 |              4.4 |               1.5 |              0.4 |     setosa |             setosa             |
|               5.4 |              3.9 |               1.3 |              0.4 |     setosa |             setosa             |
|               5.1 |              3.5 |               1.4 |              0.3 |     setosa |             setosa             |
|               5.7 |              3.8 |               1.7 |              0.3 |     setosa |             setosa             |
|               5.1 |              3.8 |               1.5 |              0.3 |     setosa |             setosa             |
|               5.4 |              3.4 |               1.7 |              0.2 |     setosa |             setosa             |
|               5.1 |              3.7 |               1.5 |              0.4 |     setosa |             setosa             |
|               4.6 |              3.6 |                 1 |              0.2 |     setosa |             setosa             |
|               5.1 |              3.3 |               1.7 |              0.5 |     setosa |             setosa             |
|               4.8 |              3.4 |               1.9 |              0.2 |     setosa |             setosa             |
|                 5 |                3 |               1.6 |              0.2 |     setosa |             setosa             |
|                 5 |              3.4 |               1.6 |              0.4 |     setosa |             setosa             |
|               5.2 |              3.5 |               1.5 |              0.2 |     setosa |             setosa             |
|               5.2 |              3.4 |               1.4 |              0.2 |     setosa |             setosa             |
|               4.7 |              3.2 |               1.6 |              0.2 |     setosa |             setosa             |
|               4.8 |              3.1 |               1.6 |              0.2 |     setosa |             setosa             |
|               5.4 |              3.4 |               1.5 |              0.4 |     setosa |             setosa             |
|               5.2 |              4.1 |               1.5 |              0.1 |     setosa |             setosa             |
|               5.5 |              4.2 |               1.4 |              0.2 |     setosa |             setosa             |
|               4.9 |              3.1 |               1.5 |              0.2 |     setosa |             setosa             |
|                 5 |              3.2 |               1.2 |              0.2 |     setosa |             setosa             |
|               5.5 |              3.5 |               1.3 |              0.2 |     setosa |             setosa             |
|               4.9 |              3.6 |               1.4 |              0.1 |     setosa |             setosa             |
|               4.4 |                3 |               1.3 |              0.2 |     setosa |             setosa             |
|               5.1 |              3.4 |               1.5 |              0.2 |     setosa |             setosa             |
|                 5 |              3.5 |               1.3 |              0.3 |     setosa |             setosa             |
|               4.5 |              2.3 |               1.3 |              0.3 |     setosa |             setosa             |
|               4.4 |              3.2 |               1.3 |              0.2 |     setosa |             setosa             |
|                 5 |              3.5 |               1.6 |              0.6 |     setosa |             setosa             |
|               5.1 |              3.8 |               1.9 |              0.4 |     setosa |             setosa             |
|               4.8 |                3 |               1.4 |              0.3 |     setosa |             setosa             |
|               5.1 |              3.8 |               1.6 |              0.2 |     setosa |             setosa             |
|               4.6 |              3.2 |               1.4 |              0.2 |     setosa |             setosa             |
|               5.3 |              3.7 |               1.5 |              0.2 |     setosa |             setosa             |
|                 5 |              3.3 |               1.4 |              0.2 |     setosa |             setosa             |
|                 7 |              3.2 |               4.7 |              1.4 | versicolor |           virginica            |
|               6.4 |              3.2 |               4.5 |              1.5 | versicolor |           versicolor           |
|               6.9 |              3.1 |               4.9 |              1.5 | versicolor |           virginica            |
|               5.5 |              2.3 |                 4 |              1.3 | versicolor |           versicolor           |
|               6.5 |              2.8 |               4.6 |              1.5 | versicolor |           versicolor           |
|               5.7 |              2.8 |               4.5 |              1.3 | versicolor |           versicolor           |
|               6.3 |              3.3 |               4.7 |              1.6 | versicolor |           virginica            |
|               4.9 |              2.4 |               3.3 |                1 | versicolor |           versicolor           |
|               6.6 |              2.9 |               4.6 |              1.3 | versicolor |           versicolor           |
|               5.2 |              2.7 |               3.9 |              1.4 | versicolor |           versicolor           |
|                 5 |                2 |               3.5 |                1 | versicolor |           versicolor           |
|               5.9 |                3 |               4.2 |              1.5 | versicolor |           versicolor           |
|                 6 |              2.2 |                 4 |                1 | versicolor |           versicolor           |
|               6.1 |              2.9 |               4.7 |              1.4 | versicolor |           versicolor           |
|               5.6 |              2.9 |               3.6 |              1.3 | versicolor |           versicolor           |
|               6.7 |              3.1 |               4.4 |              1.4 | versicolor |           versicolor           |
|               5.6 |                3 |               4.5 |              1.5 | versicolor |           versicolor           |
|               5.8 |              2.7 |               4.1 |                1 | versicolor |           versicolor           |
|               6.2 |              2.2 |               4.5 |              1.5 | versicolor |           versicolor           |
|               5.6 |              2.5 |               3.9 |              1.1 | versicolor |           versicolor           |
|               5.9 |              3.2 |               4.8 |              1.8 | versicolor |           virginica            |
|               6.1 |              2.8 |                 4 |              1.3 | versicolor |           versicolor           |
|               6.3 |              2.5 |               4.9 |              1.5 | versicolor |           versicolor           |
|               6.1 |              2.8 |               4.7 |              1.2 | versicolor |           versicolor           |
|               6.4 |              2.9 |               4.3 |              1.3 | versicolor |           versicolor           |
|               6.6 |                3 |               4.4 |              1.4 | versicolor |           versicolor           |
|               6.8 |              2.8 |               4.8 |              1.4 | versicolor |           virginica            |
|               6.7 |                3 |                 5 |              1.7 | versicolor |           virginica            |
|                 6 |              2.9 |               4.5 |              1.5 | versicolor |           versicolor           |
|               5.7 |              2.6 |               3.5 |                1 | versicolor |           versicolor           |
|               5.5 |              2.4 |               3.8 |              1.1 | versicolor |           versicolor           |
|               5.5 |              2.4 |               3.7 |                1 | versicolor |           versicolor           |
|               5.8 |              2.7 |               3.9 |              1.2 | versicolor |           versicolor           |
|                 6 |              2.7 |               5.1 |              1.6 | versicolor |           virginica            |
|               5.4 |                3 |               4.5 |              1.5 | versicolor |           versicolor           |
|                 6 |              3.4 |               4.5 |              1.6 | versicolor |           versicolor           |
|               6.7 |              3.1 |               4.7 |              1.5 | versicolor |           virginica            |
|               6.3 |              2.3 |               4.4 |              1.3 | versicolor |           versicolor           |
|               5.6 |                3 |               4.1 |              1.3 | versicolor |           versicolor           |
|               5.5 |              2.5 |                 4 |              1.3 | versicolor |           versicolor           |
|               5.5 |              2.6 |               4.4 |              1.2 | versicolor |           versicolor           |
|               6.1 |                3 |               4.6 |              1.4 | versicolor |           versicolor           |
|               5.8 |              2.6 |                 4 |              1.2 | versicolor |           versicolor           |
|                 5 |              2.3 |               3.3 |                1 | versicolor |           versicolor           |
|               5.6 |              2.7 |               4.2 |              1.3 | versicolor |           versicolor           |
|               5.7 |                3 |               4.2 |              1.2 | versicolor |           versicolor           |
|               5.7 |              2.9 |               4.2 |              1.3 | versicolor |           versicolor           |
|               6.2 |              2.9 |               4.3 |              1.3 | versicolor |           versicolor           |
|               5.1 |              2.5 |                 3 |              1.1 | versicolor |           versicolor           |
|               5.7 |              2.8 |               4.1 |              1.3 | versicolor |           versicolor           |
|               6.3 |              3.3 |                 6 |              2.5 |  virginica |           virginica            |
|               5.8 |              2.7 |               5.1 |              1.9 |  virginica |           virginica            |
|               7.1 |                3 |               5.9 |              2.1 |  virginica |           virginica            |
|               6.3 |              2.9 |               5.6 |              1.8 |  virginica |           virginica            |
|               6.5 |                3 |               5.8 |              2.2 |  virginica |           virginica            |
|               7.6 |                3 |               6.6 |              2.1 |  virginica |           virginica            |
|               4.9 |              2.5 |               4.5 |              1.7 |  virginica |           versicolor           |
|               7.3 |              2.9 |               6.3 |              1.8 |  virginica |           virginica            |
|               6.7 |              2.5 |               5.8 |              1.8 |  virginica |           virginica            |
|               7.2 |              3.6 |               6.1 |              2.5 |  virginica |           virginica            |
|               6.5 |              3.2 |               5.1 |                2 |  virginica |           virginica            |
|               6.4 |              2.7 |               5.3 |              1.9 |  virginica |           virginica            |
|               6.8 |                3 |               5.5 |              2.1 |  virginica |           virginica            |
|               5.7 |              2.5 |                 5 |                2 |  virginica |           virginica            |
|               5.8 |              2.8 |               5.1 |              2.4 |  virginica |           virginica            |
|               6.4 |              3.2 |               5.3 |              2.3 |  virginica |           virginica            |
|               6.5 |                3 |               5.5 |              1.8 |  virginica |           virginica            |
|               7.7 |              3.8 |               6.7 |              2.2 |  virginica |           virginica            |
|               7.7 |              2.6 |               6.9 |              2.3 |  virginica |           virginica            |
|                 6 |              2.2 |                 5 |              1.5 |  virginica |           versicolor           |
|               6.9 |              3.2 |               5.7 |              2.3 |  virginica |           virginica            |
|               5.6 |              2.8 |               4.9 |                2 |  virginica |           virginica            |
|               7.7 |              2.8 |               6.7 |                2 |  virginica |           virginica            |
|               6.3 |              2.7 |               4.9 |              1.8 |  virginica |           virginica            |
|               6.7 |              3.3 |               5.7 |              2.1 |  virginica |           virginica            |
|               7.2 |              3.2 |                 6 |              1.8 |  virginica |           virginica            |
|               6.2 |              2.8 |               4.8 |              1.8 |  virginica |           virginica            |
|               6.1 |                3 |               4.9 |              1.8 |  virginica |           virginica            |
|               6.4 |              2.8 |               5.6 |              2.1 |  virginica |           virginica            |
|               7.2 |                3 |               5.8 |              1.6 |  virginica |           virginica            |
|               7.4 |              2.8 |               6.1 |              1.9 |  virginica |           virginica            |
|               7.9 |              3.8 |               6.4 |                2 |  virginica |           virginica            |
|               6.4 |              2.8 |               5.6 |              2.2 |  virginica |           virginica            |
|               6.3 |              2.8 |               5.1 |              1.5 |  virginica |           virginica            |
|               6.1 |              2.6 |               5.6 |              1.4 |  virginica |           virginica            |
|               7.7 |                3 |               6.1 |              2.3 |  virginica |           virginica            |
|               6.3 |              3.4 |               5.6 |              2.4 |  virginica |           virginica            |
|               6.4 |              3.1 |               5.5 |              1.8 |  virginica |           virginica            |
|                 6 |                3 |               4.8 |              1.8 |  virginica |           virginica            |
|               6.9 |              3.1 |               5.4 |              2.1 |  virginica |           virginica            |
|               6.7 |              3.1 |               5.6 |              2.4 |  virginica |           virginica            |
|               6.9 |              3.1 |               5.1 |              2.3 |  virginica |           virginica            |
|               5.8 |              2.7 |               5.1 |              1.9 |  virginica |           virginica            |
|               6.8 |              3.2 |               5.9 |              2.3 |  virginica |           virginica            |
|               6.7 |              3.3 |               5.7 |              2.5 |  virginica |           virginica            |
|               6.7 |                3 |               5.2 |              2.3 |  virginica |           virginica            |
|               6.3 |              2.5 |                 5 |              1.9 |  virginica |           virginica            |
|               6.5 |                3 |               5.2 |                2 |  virginica |           virginica            |
|               6.2 |              3.4 |               5.4 |              2.3 |  virginica |           virginica            |
|               5.9 |                3 |               5.1 |              1.8 |  virginica |           virginica            |

```python
corrects = dataset_test.loc[dataset_test['class'] == dataset_test['predicted class (by predict())']].shape[0]
print('Prediksi Training Bayes: %d of %d == %f %%' % (corrects, len(data), corrects / len(data) * 100))
```

```python
Prediksi Training Bayes: 140 of 150 == 93.333333 %
```