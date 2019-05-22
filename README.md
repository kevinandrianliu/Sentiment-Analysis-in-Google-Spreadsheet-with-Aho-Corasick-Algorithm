# Sentiment Analysis in Google Spreadsheet with Aho-Corasick Algorithm
### **_(Ubah file README.md ini setelah program diselesaikan)_**

## Latar Belakang
Kalian sudah pernah mengisi bit.ly/buatstima belum? Jika belum, tolong diisi ya(\*berharap). Meskipun kalian harus mengisinya pakai email std, tapi aku jamin bahwa tidak ada satu asistenpun yang bisa lihat siapa yang memberikan kritik dan saran tersebut. Eh, kok malah bahas ini *sih*?  
  
*Anyway*, salah seorang dari asisten tersebut, sebut saja koordasnya, melihat ada sentimen tertentu dari mahasiswa/-i peserta IF 2211 Strategi Algoritma kepada setiap asistennya. Namun, karena ia malas membaca setiap detil dari kritik dan saran yang diberikan, ia meminta kepada setiap dari kalian untuk memberitahukan siapa asisten yang memiliki sentimen tertentu.

## Spesifikasi
1. Program dibuat dalam bahasa **_Scala_** dan/atau **_Clojure_** dengan nama program ```AhoCorasick_<NIM>.scala``` untuk Scala dan ```AhoCorasick_<NIM>.clj``` untuk Clojure.  
  
2. Program akan membaca *sheet* yang akan diberikan ketika demo(silahkan gunakan *sheet dummy* dalam pengerjaan tugas ini). Diperbolehkan untuk menggunakan *library* dari luar. Sheet akan terdiri dari sebuah tabel yang berisi nomor, dan nama setiap asisten(total ada 9 kolom) dengan jumlah baris sebanyak ```N```(total ada M\*N kalimat).
  
3. Program menerima masukan dari *terminal* berupa ```M``` buah kata yang dijadikan bahan untuk sentimen analisis dipisahkan dengan spasi. Contohnya adalah ```baik jahat wibu```. 
  
4. Lalu, program akan menggunakan algoritma Aho-Corasick untuk menentukan jumlah setiap kata pada setiap asisten. Misalkan kata yang menjadi sentimen analisis adalah *baik* dan *jahat*, maka format tampilannya adalah sebagai berikut:
```
Kevin  
Baik : <jumlah kata baik pada bagian Kevin>  
Jahat : <jumlah kata baik pada bagian Kevin>  
Total : <total>  
  
Rabbi  
Baik : <jumlah kata baik pada bagian Rabbi>  
Jahat : <jumlah kata baik pada bagian Rabbi>  
Total : <total>  
```  
dan seterusnya. Lalu, akan ditentukan asisten yang memiliki total terbesar dengan format keluaran sebagai berikut:  
```  
Maka, <nama> yang memiliki sentimen <daftar kata> paling banyak.  
```  
5. Batasan kasus uji : 1 <= M <= 10 dan 1 <= N <= 75. Setiap kalimat memiliki rentang dari 1-60 kata.
  
6.	Program memiliki *Readme* yang berisi:
- *Environment* pembuatan program(termasuk *library* yang digunakan)
- Asumsi dalam pembuatan program(jika ada)
- Deskripsi algoritma yang digunakan
- Cara menggunakan program
- Data diri
  
7. **_Program harus ditulis dengan menggunakan nama-nama variabel, fungsi, dan prosedur yang dapat dimengerti. Program perlu memasukkan komentar pada beberapa bagian yang mungkin tidak mudah ditangkap dengan baik oleh saya._**  
  
8. **_Jika memiliki asumsi, tanyakan terlebih dahulu kepada saya. Asumsi yang dituliskan dalam *Readme* adalah setiap pertanyaan yang saya jawab, “Asumsikan sendiri.”_**  
  
9. **_Penilaian tugas ini dalam bentuk fitur-fitur, sehingga jika ada yang ingin mengirimkan program yang tidak lengkap, silahkan dikumpulkan saja._**  
 

## Penilaian
1. Fitur yang diuji adalah sebagai berikut:
- Pembacaan *sheet*
- Pembacaan masukan daftar kata dari terminal
- Algoritma Aho-Corasick
- Bonus
  
2. Pengerjaan dengan **_Scala_** akan diberi nilai **_2400_**, sedangkan jika menambah implementasi dengan **_Clojure_** akan menambah bonus **_1500_**.

3. **_Penilaian akan digunakan dengan sheet asli dari bit.ly/buatstima, sehingga silahkan siapkan semua kemungkinan yang mungkin. Dipastikan bahwa semua karakter yang dipakai dalam pengujian adalah karakter ASCII. Sheet dummy merupakan bantuan untuk kalian agar tidak ada data yang bocor sebelum demo_**
