<h1> Gameobject, Component, Canvas & UI </h1>
<p> oleh Felix Irwanto (GameDev Kelompok 3) </p>
<br>

## Gameobject

<p align="center"><img width="100%" src=""> </p>

***Gameobject*** adalah .

<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/113922230/192142768-6c0c8fe5-4a23-45cb-987b-ddb4177b41a6.png"> </p>

***Unity Hub*** adalah software tambahan yang ikut didownload ketika ingin mendownload unity. Unity Hub berfungsi melanjutkan development sebuah projek (game) dalam versi unity yang berbeda.

<h2>Camera</h2>

<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192145244-1b3c5ac8-3642-42b6-8d14-e229071d1fb2.png"> </p>

***Camera*** adalah semua hal yang ada pada game dilihat dari sudut pandang arah mata pengguna yang menangkap semua gambaran yang mengarah kepadanya. Terdapat beberapa property camera seperti gambar berikut: 

<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/113922230/192149445-adcfd0fa-ac84-4d33-9489-2427e8cca8b5.png"> </p>

<h2>Scene Window</h2>

<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192146088-9ad2bbe3-1033-47fe-96b5-4738093f40c1.png"> </p>

***Scene Window*** adalah tempat letak semua tampilan game (dunia dalam game). Scene Window bisa terdiri dari beberapa halaman dan kita dapat mengutak-atik semua objek yang ada. Contoh: Level game (1 level game = 1 scene), meja, dll.

<h2>Hierarchy Window</h2>

<p align="center"><img width="50%" src="https://user-images.githubusercontent.com/113922230/192146061-118a9291-db2d-45ac-bfaa-00bdcdfd3ecc.png"> </p>

***Hierarchy Window*** adalah otak dari semua objek. Pada default, terdapat Main Camera dan Directional Light. Hal yang dapat dilakukan seperti membuat, menghapus, menduplikat gameobject, mengatur keterlihatan dari gameobject, merapikan, menyusun, dam mengelompokkan gameobject.

<h2>Console Window</h2>

<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192148963-552c2b6a-7aa3-4b78-8028-614b80cbf7e1.png"> </p>

***Console Window*** adalah tampilan jendela yang memberikan pesan peringatan, error, dan semua pesan dari editor. Berbeda dengan console lain, console window di Unity tidak dapat membaca input (hanya menampilkan output). Hanya digunakan pada saat pengembangan. Opsi toolbar yang ada, seperti clear, collapse, dan error pause.

<h2>Project</h2>

<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192146663-a9743f20-3f89-430a-9b40-891a8556fa74.png"> </p>

***Project*** adalah tempat penyimpanan semua file dari sebuah projek di Unity. Pada file manager di desktop, folder projek dikenal dengan nama "Assets". 

<h2>Hello World (Scripting)</h2>

<p align="center"><img width="100%" src=""> </p>

***Scripting*** adalah unsur penting dalam Unity. Scripting berguna untuk menanggapi masukan dari pemain dan mengatur agar peristiwa dalam gameplay terjadi saat seharusnya. Selain itu, skrip dapat digunakan untuk membuat efek grafis, mengontrol perilaku fisik objek, atau bahkan menerapkan sistem AI khusus untuk karakter dalam game. 

Tahapan untuk dapat melakukan scripting ("Hello World") di Unity:
<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192147302-4cc6f3ab-6f29-4553-a7ec-ec61122952d2.png"> </p> 

- Ke Window > Package Manager > Packages (Unity Registry)
- Pastikan Visual Scripting, VSC Code Editor, dan Visual Studio Editor telah terinstall
<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192147573-e0ee1f61-a743-4bb9-9ff1-2e790fd75401.png"> </p>

- Ke Edit > Preferences > External Tools > External Script Editor > Ubah menjadi Visual Studio Code
- Lalu, Project > Assets > Create > Folder (biar rapi) > C# Scripts

<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192148478-149c90f9-6b2d-4c32-8b4f-3ff177f5c96a.png"> </p>

- Unity > Hierarchy > Create Empty > Add Component > Script "Hello World"
Source Code:
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class HelloWorld : MonoBehaviour
{
    // Start is called before the first frame update
    void Start()
    {
        Debug.Log("Hello World");
        Debug.LogWarning("Log");
        Debug.LogError("Log");
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}
```
Output:
<p align="center"><img width="100%" src="https://user-images.githubusercontent.com/113922230/192148884-5dc3d474-07cb-4c21-9e6b-4e0e1eae9aab.png"> </p>

<br/>
**Copyright by Felix Irwanto - 2022**
