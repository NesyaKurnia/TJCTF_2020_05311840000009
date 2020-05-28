

# Ling Ling

## Soal
Who made this [meme](https://static.tjctf.org/d25fe79e6276ed73a0f7009294e28c035437d7c7ffe2f46285e9eb5ac94b6bec_meme.png)? [I made this meme](https://www.reddit.com/r/lingling40hrs/comments/gam2if/this_popped_in_my_mind_as_i_was_playing_it_and_i/)! unless.....

![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Forensics/Ling%20Ling/meme.png)

## Penyelesaian
Setelah mengunduh gambar yang ada pada soal, dapat dilihat gambar tersebut adalah meme dengan not balok __Chopins Third Ballade__. <br> Dari soal dapat diketahui yang dicari adalah __Artist/pembuat__ dari meme tersebut. Untuk mendapatkan data tersebut dapat menggunakan `exiftool` dan grep pada terminal. 
```
$ exiftool meme.png | grep Artist
```
  
Setelah itu akan muncul langsung __Artist/pembuat__ dari meme tersebut.

## FLAG
__`tjctf{ch0p1n_fl4gs}`__
