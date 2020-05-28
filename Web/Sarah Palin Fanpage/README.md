# Sarah Palin Fanpage

## Soal 
Are you a true fan of Alaska's most famous governor? Visit the [Sarah Palin fanpage](http://sarah_palin_fanpage.tjctf.org/).

## Penyelesaian
Kita akan masuk ke website [Sarah Palin Fanpage](http://sarah_palin_fanpage.tjctf.org/). Pada web Sarah tersebut kita melihat ada tab `Home`, `Top 10 moments`, `VIP area`, dan `About`.
- `flag` berada pada `VIP area`. 
<br> Untuk mengakses VIP area, kita harus mengubah _value_ dari __data__ yang terdapat pada cookies
- Pertama kita harus melakukan inspect elements dengan menekan tombol F12.
- Kemudian buka bagian _Application_ dan buka cookie. Disana terlihat ada __data__ dengan value :`eyIxIjpmYWxzZSwiMiI6ZmFsc2UsIjMiOmZhbHNlLCI0IjpmYWxzZSwiNSI6ZmFsc2UsIjYiOmZhbHNlLCI3IjpmYWxzZSwiOCI6ZmFsc2UsIjkiOmZhbHNlLCIxMCI6ZmFsc2V9` 
- Value ini akan kita decode menggunakan __base64__ [online tools](https://www.base64decode.org/) sehingga outpunya menjadi `{"1":false,"2":false,"3":false,"4":false,"5":false,"6":false,"7":false,"8":false,"9":false,"10":false}`. 
![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Web/Sarah%20Palin%20Fanpage/Decode.png)
<br> Kemudian __false__ diubah menjadi __true__
- Setelah diubah menjadi __true__, kita melakukan encode dengan menggunakan [online tools](https://www.base64encode.org/) yang akan menghasilkan output `eyIxIjp0cnVlLCIyIjp0cnVlLCIzIjp0cnVlLCI0Ijp0cnVlLCI1Ijp0cnVlLCI2Ijp0cnVlLCI3Ijp0cnVlLCI4Ijp0cnVlLCI5Ijp0cnVlLCIxMCI6dHJ1ZX0=`
![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Web/Sarah%20Palin%20Fanpage/Encode.png)
- Hasil encode diatas, kita masukkan lagi pada value data yang terdapat pada cookies
- Kemudian lakukan refresh pada halaman web, dan pada tab __VIP area__ akan terdapat flag

## FLAG
Flag ini didapatkan setelah perubahan soal dilakukan :
__`tjctf{wkDd2Pi4rxiRaM5lOcLo979rru8MFqVHKdTqPBm4k3iQd8n0sWbBkOfuq9vDTGN9suZgYlH3jq6QTp3tG3EYapzsTHL7ycqRTP5Qf6rQSB33DcQaaqwQhpbuqPBm4k3iQd8n0sWbBkOf}`__
