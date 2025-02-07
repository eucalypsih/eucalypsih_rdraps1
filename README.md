## powi
fungsi powi di Rust digunakan untuk menghitung pangkat dari sebuah bilangan dengan eksponen yang merupakan bilangan bulat (integer). Fungsi ini biasanya digunakan dalam konteks matematika dan pemrograman numerik, di mana Anda perlu melakukan operasi pangkat dengan eksponen yang tidak berubah.
* Menghitung Kuadrat: Anda dapat menggunakan powi untuk menghitung kuadrat dari sebuah bilangan.
* Menghitung Pangkatan Negatif: Anda dapat menggunakan eksponen negatif untuk menghitung invers dari bilangan.


## ln
fungsi log di Rust digunakan untuk menghitung logaritma dari sebuah bilangan floating-point. Fungsi ini tersedia untuk tipe data f32 dan f64, dan dapat digunakan untuk menghitung logaritma dengan basis tertentu.
* Logaritma Natural (Basis e): Untuk menghitung logaritma natural (basis e), Anda dapat menggunakan metode ln().


## result
Kesimpulan: Tipe Result di Rust adalah alat yang sangat berguna untuk menangani kesalahan dengan cara yang aman dan eksplisit. Dengan menggunakan Result, Anda dapat meningkatkan kejelasan kode, mendorong penanganan kesalahan yang tepat, dan menghindari kesalahan yang tidak terduga di runtime. Ini adalah salah satu fitur yang membuat Rust menjadi bahasa yang kuat dan aman untuk pengembangan perangkat lunak.

Rust menyediakan beberapa metode berguna untuk bekerja dengan `Result`
* `is_ok()`: Mengembalikan true jika hasilnya adalah `Ok`.
* `is_err()`: Mengembalikan true jika hasilnya adalah `Err`.
* `unwrap()`: Mengambil nilai dari Ok, tetapi akan panik jika hasilnya adalah `Err`.
* `expect(msg)`: Mirip dengan `unwrap()`, tetapi memungkinkan Anda untuk memberikan pesan kesalahan yang lebih informatif.
* `map()`: Mengubah nilai dalam `Ok` jika ada, dan tetap mempertahankan `Err`.
* `and_then()`: Menggunakan hasil dari `Ok` untuk menghasilkan `Result` baru.
* `unwrap_or(default)`: Mengembalikan nilai dari `Ok`, atau nilai default jika hasilnya adalah `Err`.


## string
* `trim()`: Untuk menghapus spasi di awal dan akhir string.
* `format!()`: Untuk menggabungkan string dengan cara yang lebih fleksibel.
* `contains()`: Memeriksa apakah string mengandung substring tertentu.
* `as_str()`: Anda dapat mendapatkan referensi &str dari String menggunakan metode as_str.












## eof
