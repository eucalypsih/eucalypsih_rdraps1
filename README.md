## powi
fungsi powi di Rust digunakan untuk menghitung pangkat dari sebuah bilangan dengan eksponen yang merupakan bilangan bulat (integer). Fungsi ini biasanya digunakan dalam konteks matematika dan pemrograman numerik, di mana Anda perlu melakukan operasi pangkat dengan eksponen yang tidak berubah.
* Menghitung Kuadrat: Anda dapat menggunakan powi untuk menghitung kuadrat dari sebuah bilangan.
* Menghitung Pangkatan Negatif: Anda dapat menggunakan eksponen negatif untuk menghitung invers dari bilangan.


## ln
fungsi log di Rust digunakan untuk menghitung logaritma dari sebuah bilangan floating-point. Fungsi ini tersedia untuk tipe data f32 dan f64, dan dapat digunakan untuk menghitung logaritma dengan basis tertentu.
* Logaritma Natural (Basis e): Untuk menghitung logaritma natural (basis e), Anda dapat menggunakan metode ln().


## result
Rust menyediakan beberapa metode berguna untuk bekerja dengan `Result`
* `is_ok()`: Mengembalikan true jika hasilnya adalah `Ok`.
* `is_err()`: Mengembalikan true jika hasilnya adalah `Err`.
* `unwrap()`: Mengambil nilai dari Ok, tetapi akan panik jika hasilnya adalah `Err`.
* `expect(msg)`: Mirip dengan `unwrap()`, tetapi memungkinkan Anda untuk memberikan pesan kesalahan yang lebih informatif.
* `map()`: Mengubah nilai dalam `Ok` jika ada, dan tetap mempertahankan `Err`.
* `and_then()`: Menggunakan hasil dari `Ok` untuk menghasilkan `Result` baru.
* `unwrap_or(default)`: Mengembalikan nilai dari `Ok`, atau nilai default jika hasilnya adalah `Err`.
