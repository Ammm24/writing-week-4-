# java script intermediate
## Asynchronus Async Await
### Asyncronus Await
- `async` untuk mengubah function synchronus menjadi asynchronus.
- `await` untuk menunda eksekusi hingga proses asynchronus selesai.
### Cara menghandel eror async await
Untuk menghandle error  Async/Await kita dapat menggunakan try catch di dalam function yang kita buat, sehingga jika terjadi error kita dapat menangkap errornya dalam block catch, berikut contoh penggunaannya.
```javascript
const getAllUser = async ()=> {
	try {
		const result = await getUser()
		console.log(result)
	} catch (error) {
		console.log(error)
	}
}
```
### Asyncronus fetch
Fetch API pada javascript adalah kegiatan untuk meminta/request layanan ke endpoint/letak url yang akan menerima request pada website secara local maupun public, untuk mengambil response resource / sumber daya berupa data berformat json atau text yang biasa dilakukan programmer untuk membangun website yang membutuhkan data dari website lain ataupun website yang membutuhkan konsep microservice didalamnya.
- fetch dengan promise
```javascript
fetch("https://jsonplaceholder.typicode.com/posts") //menghubungkan dengan api melalui url
  .then(function (response) {
    return response.json(); // .json() untuk unboxing data json
  })
  .then(function (post) {
    console.log(post);
  });
  ```
  - fetch dengan async await
  ```javascript
  const tesFetchAsync = async () => {
  let response = await fetch("https://jsonplaceholder.typicode.com/posts");
  response = await response.json();
  console.log(response);
};
tesFetchAsync();
```
## Git dan github lanjutan 
- Git adalah version control system, sedangkan GitHub adalah code repository and sharing platform
- GitHub adalah tempat untuk menyimpan kode di cloud serta tempat untuk berbagi dan berkolaborasi dengan orang lain.

Dengan Git dan GitHub kita bisa melakukan kolaborasi atau bekerja di dalam sebuah tim saat pengerjaan sebuah tim. Beberapa perintah yang digunakan untuk melakukan kolaborasi :
- git clone untuk mengcopy semua repository pada github ke dalam komputer kita, dengan cara mengclone pada link github repository
- git pull untuk mengupdate kode yang telah kita buat 
- git branch [nama-branch] untuk membuat branch baru dimana setiap anggota kelompok akan mengerjakan tugasnya masing-masing.
- git merge [nama-branch] untuk menggabungkan branch yang aktif dan branch yang dipilih.
- Beberapa command dasar seperti git commit, git add, git push, dll.

## Responsive web 
Responsive Web Design adalah suatu keadaan sebuah halaman web dimana tampilannya akan cocok, rapi dan tetap enak dilihat jika diakses dari perangkat apapun dengan resolusi layar yang berbeda. Misalnya, ketika anda mengakses blog ini dengan perangkat (PC/HP/Tablet) yang berbeda, anda akan melihat tampilannya berbeda karena menyesuaika dengan layar. Secara umum, sebuah halaman web tidak bisa menyesuaikan tampilannya sendiri dengan resolusi layar perangkat yang mengaksesnya.

Responsive Design dikembangkan melalui kode-kode CSS seperti dibawah ini 
```javascript
@media(min-width:992px) {
       .selector { 
             width:970px; 
        }
} 

@media(max-width:768px) {
        .selector { 
              width:750px;
        }
}
```
## BOOTSTRAP 5
Bootstrap merupakan framework untuk membangun desain web secara responsif. Artinya, tampilan web yang dibuat oleh bootstrap akan menyesuaikan ukuran layar dari browser yang kita gunakan baik di desktop, tablet ataupun mobile device.

Bootstrap memiliki banyak kegunaan yang membuat kita menjadi lebih cepat untuk membuat sebuah komponen website, seperti saat ingin membuat navigasi bar, kita tinggal melihat Components, pilih Navbar, selanjutnya adalah tinggal pilih navigasi bar yang sesuai dengan kebutuhan kita, setelah itu tinggal copy source codenya dan paste ke dalam file HTML kita dan kita bisa modifikasi konten dari navigasi tersebut sesuai dengan kebutuhan kita.
### Kelebihan dalam memakai bootsrap 
1. Ramah untuk pemula
2. Grid System yang Canggih
3. Kompatibilitas dengan Web Browser Terbaru
4. Bersifat Open-Source
5. Kebebasan Kustomisasi
6. Rutin Diperbarui
7. Tersedia Dokumentasi Lengkap
8. Memiliki Komunitas Besar yang Aktif
### Kekurangan dalam memakai bootstrap
1. Elemennya Banyak Digunakan Developer Website Lain
2. Bisa Memperlambat Website
3. Memperlambat Proses Belajar
