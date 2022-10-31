
# **Presentasi-minggu-6**

## **Intro React JS** 
React JS  merupakan sebuah javascript library yang dibuat oleh facebook yang memiliki sifat composable atau bisa dibilang dalam pembuatan UI, kita dapat bagi menjadi beberapa komponen. React JS sedikit berbeda dengan vanilla javascript karena pada React JS kita tidak menggunakan DOM melainkan virtual DOM. Virtual DOM ini bisa dibilang sebuah versi *light* nya karena virtual DOM hanya meng-update bagian yang diperlukan sehingga waktu yang dibutuhkan lebih singkat. 
### Instalasi React JS
Berikut ini merupakan tahapan yang harus di lakukan dimana terbagi menjadi 2 bagian, instalasi Node JS dan instalasi proyek nya: 
A. Instalasi Node JS
1.  Download Node JS [https://nodejs.org/en/download]
![enter image description here](https://i.postimg.cc/85T5s5sd/image.png)

3.  Check Node dan NPM

```
      node --version (untuk melihat 
      npm --version
```

3.Install Create React App Library

```
        npm install -g create-react-app
```

B. Instalasi Proyek react JS
1.  Buka Terminal atau Gitbash kemudian beri perintah :

```
    npx create-react-app [name-project]
```
2.  Kemudian pindah direktori menuju folder react yang telah kita buat
```
	cd [name-project] 
```
3. Terakhir untuk menjalankan react JS tersebut gunakan perintah dibawah ini
```
    npm run start
```
## **Functional Component, Props dan State** 

![enter image description here](https://i.postimg.cc/VvHmByc5/image.png)

### **Component**

Component merupakan sebuah separate-part yang bersifat re-usable. Sebenarnya secara konseptual component pada react js merupakan sebuah function, karena reactjs menggunakan virtual DOM nah component inilah yang memiliki fungsi untuk memberi tahu apa-apa saja yang nanti nya akan di render ke real DOM. Implementasi component adalah ketika kita ingin membuat sebuah fitur pada website kita hanya perlu membuat file .jsx baru dengan export default kemudian import component tersebut ke file app.jsx utama
_Note : penggunaan nama function di React JS harus diawali Huruf Besar_

![enter image description here](https://i.postimg.cc/N0PHV8GN/image.png)

Berdasarkan definisi dimana React JS merupakan library berbasis component Based, React JS terbagi menjadi 2 bagian, yaitu class component dan functional component.

1.  **Class Component**

> Contoh penulisan class component
![enter image description here](https://i.postimg.cc/mDKR0kHf/image.png)

2.  **Functional Component**

> Penulisan functional component ada 2, yaitu function biasa dan arrow function

 -   Function biasa
 ![enter image description here](https://i.postimg.cc/Y9zfPGVj/image.png)
 -   Arrow function
   ![enter image description here](https://i.postimg.cc/vDFY6TYL/image.png)
    

*Note :*

 - Tiap component yang dibuat harus diberikan export default [nama_fungsi] pada akhirnya kemudian import kedalam App.jsx 
  - Proses render hanya dilakukan untuk satu element maka dari itu segala logic yang dibuat ditaruh didalam `<div></div>`
   
### Props

Props merupakan sebuah object yang berisi data dari komponen lain. 
![enter image description here](https://i.postimg.cc/jjtjXMVV/image.png)
### State
State merupakan sebuah object yang berisi data dari lokal sebuah komponen.
![enter image description here](https://i.postimg.cc/0jYkDSt5/image.png) 
## **Event-Handling dan Conditional Rendering** 
### Event-handling
Pada react JS ketika ingin meng-handle sebuah event kita bisa menggunakan event listener seperti hal nya vanilla JS (onClick, onChange, onSubmit.. dan lainnya). 

![enter image description here](https://i.postimg.cc/YSmD8BF0/image.png)
### Conditional Rendering
Conditional rendering pada React JS sebenarnya sama penggunaan nya seperti pada vanilla javascript yaitu membuat sebuah kondisi dimana ketika kondisi tersebut terpenuhi maka React akan men-update nya

![enter image description here](https://i.postimg.cc/3rFTTmc1/image.png)
## **Lifecycle dan Hooks** 
### Lifecycle
Lifecycle adalah sebuah method yang digunakan ketika ingin mendevelop sebuah website. Lifecycle sendiri memiliki 3 proses utama yaitu mounting (insert element kedalam DOM), updating (update element kedalam DOM) dan unmounting (me-remove element dari DOM). 

![enter image description here](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSd39db6i6IoWg8i7wOSmB5xwT3uE4_AS_BWw&usqp=CAU)
### Hooks
Hooks pada React.js merupakan sebuah function yang dapat digunakan pada functional component seperti useState, useEffect, useContext, useReducer, useCallback dan lainnya.  Kalau useState digunakan untuk membuat state di function komponen, useEffect digunakan untuk menambahkan side effect ke function komponen. UseEffect memiliki ciri" yaitu terdapat dua parameter dimana parameter pertama yaitu sebuah callback dan kedua berupa array (depedensi). contoh implementasi nya adalah : 
![enter image description here](https://i.postimg.cc/656DNQgG/image.png)

maka ketika kita inspect urutan yang akan muncul pada console adalah 
1. ini sebelum return 
 2. ini return 
2. ini dari use effect setelah return 
![enter image description here](https://i.postimg.cc/K8tG1jcv/image.png)
>maka kesimpulan yang bisa ditarik adalah pada proses pengeksekusian event diluar return akan dieksekusi terlebih dahulu lalu pada return dan terakhir pada useEffect. 
## **Form** 
Form pada react js dan vanilla javacript memiliki perbedaan, perbedaan tersebut yaitu ketika kita membuat form pada vanilla javascript kita maka fitur yang kita manfaat kan adalah Document Object model atau biasa disebut DOM sementara jika kita mebuat form menggunakan react js maka kita akan menggunakan component state event onChange untuk merubah data nya serta hooks dan event-handler. 
![enter image description here](https://i.postimg.cc/T3P86Py4/image.png)



