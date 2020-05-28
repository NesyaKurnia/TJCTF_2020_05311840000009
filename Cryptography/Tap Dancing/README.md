# Tap Dancing

## Soal
My friend is trying to teach me to dance, but I am not rhythmically coordinated! They sent me a list of [dance moves](https://static.tjctf.org/518d6851c71c5482dbd5bbe812b678684238c8f4e9e9b3d95a188f7db83a0870_cipher.txt) but they're all numbers! Can you help me figure out what they mean so I can learn the dance?

NOTE: Flag is not in flag format.

## Penyelesaian
Ini merupakan _list dance move_ `1101111102120222020120111110101222022221022202022211`
<br> Kode diatas harus kita terjemahkan menjadi __kode morse__ terlebih dahulu dengan ketentuan seperti dibawah ini :
<br> __0 = spasi (" ")__
<br> __1 = minus (-)__
<br> __2 = titik (.)__
<br> Hasil kode morse dari list dance move yang sudah ditentukan :
<br> `-- ----- .-. ... . -. ----- - -... ....- `
<br> Setelah menghasilkan kode morse, kita melakukan __konversi__ dari kode morse menjadi text menggunakan [translator online](https://morsify.net/), sehingga akan menemukan __flagnya__.
![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/Tap%20Dancing/convert.jpg)

## FLAG
__`tjctf{M0RSEN0TB4SE3}`__
