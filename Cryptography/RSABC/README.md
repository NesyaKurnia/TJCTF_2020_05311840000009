# RSABC

## Soal 
I was just listening to some [relaxing ASMR](https://youtu.be/J2g3lvNkAfI) when a notification popped up with [this](https://static.tjctf.org/68f148e8d4b5ceb8f9fa6da568db024c28b80b55891fba49880b76b35d436114_rsa.txt).
???

_Hint: 
It's easy as R-S-A! Wait.._

## Penyelesaian
1. Setelah mengetahui hint yang terdapat di Challenge, bisa mencari referensi pengerjaan di `TJCTF-2019 Easy as RSA`
2. Melakukan faktorisasi pada nilai __"n"__ (mendapatkan p dan q) dengan menggunakan faktorisasi online pada alamat [factordb.com](http://factordb.com/)
<br> Nilai __p__ dan __q__ yang saya dapatkan :
```
p = 202049603951664548551555274464815496697
q =  285934543893985722871321330457714807993
```
3. Selanjutnya adalah menginputkan n, e, c serta p dan q kedalam Ruby Script, seperti gambar dibawah ini :
![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/RSABC/code.jpg). Script yang digunakan adalah [solve.rb](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/RSABC/solve.rb)

4. Kemudian jalankan script `solve.rb` menggunakan command seperti dibawah ini :
```
$ ruby solve.rb
```
5. Outputnya akan tampil seperti dibawah ini :
![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/RSABC/output.jpg)

## FLAG
__`tjctf{BOLm1QMWi3c}`__