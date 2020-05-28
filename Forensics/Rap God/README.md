# Rap God

## Soal
My rapper friend Big Y sent me his [latest track](https://static.tjctf.org/302ed01b56ae5988e8b8ad8d9bba402a2934c71508593f5dc9e95aed913d20cf_BigYAudio.mp3) but something sounded a little off about it. Help me find out if he was trying to tell me something with it. Submit your answer as tjctf{message}

## Penyelesaian
- Pertama-tama, kita lakukan pengunduhan file `.mp3` dari soal tersebut.
- Dengan menggunakan aplikasi __Accoustic Spectrum Analyzer__, kita bisa melihat Spektrum Audio dari file `.mp3` tersebut. Sehingga akan menampilkan seperti gambar dibawah ini :
![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Forensics/Rap%20God/analisis%20audio.jpg)
- Pada hasil spektrum audio tersebut, dapat terlihat sebuah symbol-simbol. Simbol tersebut merupakan sebuah font yang bernama __Wingdings__ pada WORD 2003.
<br> ![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Forensics/Rap%20God/emoji%20word%202003%20yang%20digunakan%20pada%20spektrum%20audio.jpg)
- Terakhir lakukan konversi Simbol/Font tersebut menjadi huruf-huruf, maka akan didapatkannya sebuah kata yaitu `QUICKSONIC`.
- masukkan kata tersebut dalam format flag: `tjctf{QUICKSONIC}`.

## FLAG
__`tjctf{QUICKSONIC}`__
