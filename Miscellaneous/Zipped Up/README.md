# Zipped Up

## Soal
My friend changed the password of his Minecraft account that I was using so that I would stop being so addicted. Now he wants me to work for the password and sent me this  [zip file](https://static.tjctf.org/663d7cda5bde67bd38a8de1f07fb9fab9dd8dd0b75607bb459c899acb0ace980_0.zip). I tried unzipping the folder, but it just led to another zipped file. Can you find me the password so I can play Minecraft again?

## Penyelesaian
1. Lakukan pengunduhan terhadap **_zip file_** melalui terminal ubuntu dengan menggunakan ```wget``` 
	```html
	wget "https://static.tjctf.org/663d7cda5bde67bd38a8de1f07fb9fab9dd8dd0b75607bb459c899acb0ace980_0.zip"
	```	
2. Unzip pada **_zip file_** tersebut dengan melakukan klik kanan 
3. Lakukan _rename_ pada hasil unzip dengan nama lain yang lebih mudah untuk ditulis dalam metode selanjutnya.
4. Dapat kita lihat bahwa ada file ```1.tar.bz2``` di dalam folder ekstrak. <br>
5. Kita akan menggunakan sebuah **_python script_**  untuk melakukan pengekstrakan __semua file__ yang ada di dalam folder ekstrak 
	```html
	from os import system

	system('unar ./1.tar.bz2')
	for i in range(1.1000,1):
		system('unar./{}/{}.*'.format(i, i+1))
	```

6.   **_python script_** tersebut dijalankan dalam folder ekstrak.
7. Ada  __1000 folder__ dalam folder ekstrak tetapi apa isi dari setiap folder?

8. ```cat``` pada salah satu folder misalnya folder ```1```
	```html
	cat 1.txt
	```
10. Gunakan ```grep``` untuk mengetahui ```flag```
	```html
	grep -v -r "tjctf{n0t_th3_fl4g}" /home/akmu/Documents/ZippedUp/0
	```
11. Temukan ```flag``` dari hasil langkah nomor ```10```

## FLAG
__`tjctf{p3sky_z1p_f1L35}`__

