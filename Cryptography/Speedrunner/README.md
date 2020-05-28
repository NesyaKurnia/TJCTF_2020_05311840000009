# Speedrunner

## Soal
I want to make it into the hall of fame -- a top runner in "The History of American Dad Speedrunning". But to do that, I'll need to be faster. I found some [weird parts](https://static.tjctf.org/6e61ec43e56cff1441f4cef46594bf75869a2c66cb47e86699e36577fbc746ff_encoded.txt) in the American Dad source code. I think it might help me become the best. 

## Penyelesaian
1. Pencarian ```flag``` akan kita cari melalui _link_  [weird parts](https://static.tjctf.org/6e61ec43e56cff1441f4cef46594bf75869a2c66cb47e86699e36577fbc746ff_encoded.txt)  <br>  
![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/Speedrunner/text.png)
  
  <br>Darisini, kita dapat melihat dengan sangat jelas terdapat 1 (satu) kalimat dengan ```flag format```  <br>  
![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/Speedrunner/flag%20belum%20di%20encrypt.png) 
  <br>Karena ```flag``` tersebut masih belum sesuai dengan ```flag format sebenarnya``` dan terdapat __Hint__ yang menunjukkan bahwa ```flag``` di dalam _link_ berbentuk __cipher__, maka kita perlu melakukan pendeskripsian melalui _online tools for decrypt_ yakni ```Cryptii```. Jangan lupa untuk mengatur __shift__ dari __cipher__ tersebut hingga kita berhasil menemukan ```flag``` dengan ```flag format sebenarnya```<br>  
  ![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/Speedrunner/proses%20encrypt.png) 
  <br>Nah, pada bagian __plaintext__ dapat kita lihat ```flag format sebenarnya```  <br>  
  ![](https://github.com/NesyaKurnia/TJCTF_2020_05311840000009/blob/master/Cryptography/Speedrunner/FLAG.png)

## FLAG
__`TJCTF{NEW_TECH_NEW_TECH_GO_FAST_GO_FAST}`__
