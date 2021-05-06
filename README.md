# GUI-Matlab
pertama-tama buatlah sebuah guide baru kemudian buat aplikasi GUI MENAMPILKAN GAMBAR DAN URL...

berikut hasil outputnya :

![UTS GUI](https://user-images.githubusercontent.com/82009410/117353171-02528c80-aeda-11eb-803d-96bb074d854a.PNG)

berikut ini desainnya :

![berikut hasil desain](https://user-images.githubusercontent.com/82009410/117353352-375edf00-aeda-11eb-8590-02af5b85687d.PNG)

berikut codingannya :

[namafile,namapath]=uigetfile({'*.jpg';'*.*'},'ambilgambar');
ambilgambar=imread([namapath,namafile]);
set(handles.url,'string',[namapath,namafile]);
axes(handles.tempatgambar);
imshow(ambilgambar);

untuk tombol KELUAR, cukup dicodingannya tinggal kasih sintaks CLOSE; agar ketika dicoba akan langsung keluar keluar tanpa harus menekan cancel..
