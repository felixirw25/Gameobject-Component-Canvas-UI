<h1> Gameobject, Component, Canvas & UI </h1>
<p> oleh Felix Irwanto (GameDev Kelompok 3) </p>
<br>

## Gameobject & Component

<p align="center"><img width="100%" src=""> </p>

***Gameobject*** adalah objek yang memiliki ***component*** komposisi tertentu. Setiap komponen dibuat menjadi satu class dan setiap class memiliki class (variabel) lain yang juga disebut sistem modular. Contoh: Musuh dengan kemampuan yang mirip (beririsan). 

Setiap Gameobject harus memiliki setidaknya satu transform biar muncul di scene (memiliki posisi, rotasi, dan skala). Gameobject memiliki relasi parent dan child. Jika parent diberi transform, maka child juga memiliki sifat tersebut. Jika child memiliki transform, parent tidak memiliki sifat tersebut. 
Contoh Pengimplementasian:
```

```
Output:
<p align="center"><img width="100%" src=""> </p>

<h2>Canvas & UI</h2>

<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192152894-32b74726-1144-4be4-9f26-c4ed786e2a5f.png"> </p>

***UI*** adalah tampilan yang dapat berinteraksi dengan pengguna yang terdiri dari komponen-komponen, seperti layar sentuh, papan ketik, suara, dan cahaya, yang dapat diberi input, ditekan, dan digerakkan. 
***Canvas*** adalah wadah khusus untuk menaruk komponen-komponen UI di Unity. Canvas sedikit berbeda dari Gameobject karena properti yang dimiliki yaitu Rect Transform dan tidak dipengaruhi oleh posisi kamera.

<h2>Inspector Window</h2>

<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/113922230/192153211-9328a750-6ec5-4a0c-818f-650f57b5d047.png"> </p>

***Inspector Window*** adalah halaman yang berfungsi melihat dan mengedit properti dan pengaturan untuk hampir semua hal di Editor Unity, termasuk GameObjects, komponen, Aset, Material, pengaturan, serta preferensi dalam Editor.

Source Code:
```

```
Output:
<p align="center"><img width="100%" src=""> </p>

<br/>
**Copyright by Felix Irwanto - 2022**
