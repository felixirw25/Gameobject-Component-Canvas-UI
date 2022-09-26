<h1> Gameobject, Component, Canvas & UI </h1>
<p> oleh Felix Irwanto (GameDev Kelompok 3) </p>
<br>

## Gameobject & Component

<p align="center"><img width="100%" src=""> </p>

***Gameobject*** adalah objek yang memiliki ***component*** komposisi tertentu. Setiap komponen dibuat menjadi satu class dan setiap class memiliki class (variabel) lain yang juga disebut sistem modular. Contoh: Musuh dengan kemampuan yang mirip (beririsan). 

Setiap Gameobject harus memiliki setidaknya satu transform biar muncul di scene (memiliki posisi, rotasi, dan skala). Gameobject memiliki relasi parent dan child. Jika parent diberi transform, maka child juga memiliki sifat tersebut. Jika child memiliki transform, parent tidak memiliki sifat tersebut. 
Contoh Pengimplementasian:
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    [SerializeField] Vector3 arah;

    [SerializeField] Vector3 rotate;

    [SerializeField] Space space;
    
    // Start is called before the first frame update
    void Start()
    {
        
    }

    Vector3 rot;
    // Update is called once per frame
    void Update()
    {
        // transform.Translate(arah*Time.deltaTime, space);
        transform.position += arah*Time.deltaTime;
        // transform.Rotate(rotate*Time.deltaTime, space);
        // rot += rotate*Time.deltaTime;
        // transform.rotation = Quaternion.Euler(rot);

        // transform.localScale *= 1 + Time.deltaTime;
        // transform.localPosition += arah*Time.deltaTime;
    }
}
```
Output:
<p align="center"><img width="40%" src="https://user-images.githubusercontent.com/113922230/192285025-5e0d2566-1585-4ffd-9d22-48ecaa01d121.png"> &nbsp; &nbsp; <img width="40%" src="https://user-images.githubusercontent.com/113922230/192285319-e920da6e-1f4f-4b82-883e-c8b74ba4953a.png"> </p>

<h2>Inspector Window</h2>

<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/113922230/192153211-9328a750-6ec5-4a0c-818f-650f57b5d047.png"> </p>

***Inspector Window*** adalah halaman yang berfungsi melihat dan mengedit properti dan pengaturan untuk hampir semua hal di Editor Unity, termasuk GameObjects, komponen, Aset, Material, pengaturan, serta preferensi dalam Editor.

<h2>Canvas & UI</h2>

<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192152894-32b74726-1144-4be4-9f26-c4ed786e2a5f.png"> </p>

***UI*** adalah tampilan yang dapat berinteraksi dengan pengguna yang terdiri dari komponen-komponen, seperti layar sentuh, papan ketik, suara, dan cahaya, yang dapat diberi input, ditekan, dan digerakkan. 
***Canvas*** adalah wadah khusus untuk menaruk komponen-komponen UI di Unity. Canvas sedikit berbeda dari Gameobject karena properti yang dimiliki yaitu Rect Transform dan tidak dipengaruhi oleh posisi kamera.

Source Code:
```

```
Output:
<p align="center"><img width="100%" src=""> </p>

<br/>
**Copyright by Felix Irwanto - 2022**
