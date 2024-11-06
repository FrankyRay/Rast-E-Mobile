# Rast-E Mobile
Remember my Rast-E Web version that can't buy/sell something? Yeah, this mobile version same.

## Tugas 7 | QnAs

### Stateless vs Stateful Widget
Stateful Widget merupakan sebuah widget yang dapat berubah-ubah ketika user melakukan interaksi. Widget tersebut biasanya menyimpan sebuat data atau *state* yang nantinya dapat diakses untuk menjalankan kode tertentu atau mengubah tampilannya.

Stateless Widget berbanding terbalik dengan Stateful Widget. Stateless Widget merupakan sebuah widget yang static, tidak banyak perubahan atau tidak berubah sama sekali. Biasanya digunakan sebagai teks deskripsi atau sebuah ikon.

### Widget yang Digunakan
Ada beberapa widget yang digunakan pada projek ini.

1. `Icon`, digunakan untuk menampilkan sebuah ikon.
1. `Text`, digunakan untuk menampilkan sebuah teks/tulisan.
1. `ScaffoldMessenger` (`SnackBar`), digunakan untuk menampilkan sebuah pesan yang muncul dari bawah layar ketika berinteraksi dengan tombol.
1. `InkWell`, widget berbentuk persegi panjang yang dapat berinteraksi ketika ditekan.

### Fungsi `setState()`
Fungsi `setState()` sesuai dengan namanya yaitu mengubah sebuah state dari sebuah widget. Cara kerjanya berupa memberitahu framework bahwa state dari sebuah widget telah berubah, sehingga framework bisa melakukan penjadwalan (scheduling) untuk membuild dengan state baru.

Contohnya biasanya App Counter, dimana sebuah label counter akan terus bertambah ketika sebuah tombol ditekan.

### `const` vs `final`
Keyword `final` mengindikasikan bahwa variable tersebut mempunyai nilai yang sudah final dan tidak dapat diubah sama sekali ketika sudah ditetapkan. Nilai dari variable yang diberikan keyword `final` biasanya ditetapkan ketika melakukan konstruksi sebuah object.

Keword `const` digunakan untuk mendeklarasi sebuah variable secara konstan (compile-time). Berbeda dengan `final`, `const` harus dideklarasi langsung dan konstant secara compile-time.

### Implementasi "Checklist"
Selain mengikuti tata cara pada tutorial 6, ada beberapa yang perlu digali untuk mengerjakan tugas 7 ini.

Pada tugas ini, tiap tombol harus mempunyai warna yang berbeda-beda, sehingga perlu adanya perubahan pada constructor `ItemHomepage`, yaitu penambahan atribut warna. Pada `ItemCard`, penentuan latar warna tombol tersebut harus diubah menggunakan warna yang sudah ditetapkan oleh `ItemHomepage`.

Ikon juga perlu diganti. Dengan melihat pada website [Icon | Google Fonts](https://fonts.google.com/icons?icon.size=24&icon.color=%23e8eaed&icon.platform=flutter), kita dapat melihat icon-icon yang dapat digunakan dan tersedia secara langsung dari Flutter menggunakan Material UI. Salah satu ikon yang saya gunakan adalah ikon `product` yang merepresentasikan tombol "Lihat Daftar Produk."