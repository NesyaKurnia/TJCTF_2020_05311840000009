# Titanic

## Soal
I wrapped tjctf{} around the lowercase version of a word said in the 1997 film "Titanic" and created an MD5 hash of it: `e246dbab7ae3a6ed41749e20518fcecd`.

## Penyelesaian
Yang kita ketahui adalah hash MD5 tersebut berasal dari script film "Titanic". 
- Setiap katanya dibuat lowercase dan di tambah dengan tjctf{}. 
- Langkah pertama adalah mengkopi script film Titanic terlebih dahulu di [sini](http://sites.inka.de/humpty/titanic/script.html). 
- Kemudian dengan bantuan visual studio code, ubah semua menjadi lowercase, hapus `.` `,` `:` `/` , ubah spasi menjadi enter dan tambahkan tjctf{} di setiap barisnya.
- Setelah itu gunakan hashcat pada terminal dengan command sebagai berikut :
```
hashcat -m 0 hash.txt dictionary.txt
```
- `hash.txt` yang isinya hash MD5 `(e246dbab7ae3a6ed41749e20518fcecd)`
- [`dictionary.txt`](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/Titanic/dictionary.txt) merupakan daftar script dari titanic yang sudah dibuat dengan format flag, menggunakan lowercase.
<bR>Langkah selanjutnya, tekan enter dan flag akan langsung terlihat

## FLAG
__`tjctf{marlborough's}`__
