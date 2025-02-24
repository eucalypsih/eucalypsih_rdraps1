```rust
use std::io::{self, Write};

fn main() {
    // Menulis ke output standar
    print!("Hello, world!");
    
    // Memastikan bahwa output ditulis ke layar
    io::stdout().flush().unwrap();
}
```
Dalam contoh di atas, kita menggunakan `print!` untuk menulis "Hello, world!" ke output standar. Namun, karena `print!` tidak secara otomatis menulis ke output (karena menggunakan buffer), kita perlu memanggil `flush()` untuk memastikan bahwa teks tersebut muncul di layar segera.

Penjelasan:
* `io::stdout()` mengembalikan handle ke output standar.
* `flush()` dipanggil untuk memastikan bahwa semua data yang tertunda dalam buffer ditulis ke output.
* `unwrap()` digunakan untuk menangani kemungkinan kesalahan yang mungkin terjadi saat memanggil `flush()`. Dalam contoh ini, kita mengabaikan kesalahan, tetapi dalam aplikasi nyata, Anda mungkin ingin menangani kesalahan dengan cara yang lebih baik.

Catatan:
* Pastikan untuk mengimpor modul yang diperlukan (std::io::{self, Write}) agar dapat menggunakan `flush()`.
* `flush()` biasanya digunakan dalam konteks di mana Anda ingin memastikan bahwa output ditampilkan kepada pengguna pada waktu tertentu, seperti dalam aplikasi interaktif.

* `bytes()`: Mengembalikan iterator yang menghasilkan byte dari string.into_bytes(): Mengonversi String menjadi `Vec<u8>`, mengkonsumsi string tersebut.
* `from_utf8()`: Mengonversi slice byte menjadi string, dengan validasi UTF-8.
* `from_utf8_lossy()`: Mengonversi slice byte menjadi String, menggantikan byte yang tidak valid dengan karakter pengganti (U+FFFD).
* `as_mut_bytes(): Mengonversi string slice menjadi mutable byte slice, memungkinkan modifikasi langsung pada data byte.
* `from_utf16()`: Mengonversi vektor yang berisi data UTF-16 menjadi String, dengan validasi untuk memastikan data yang diberikan valid.
* `from_utf8_unchecked()`: Mengonversi vektor byte menjadi String tanpa memeriksa validitas UTF-8, sehingga harus digunakan dengan hati-hati.

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


## string_kesimpulan
Dalam Rust, as_str() dan into_owned() adalah dua metode yang digunakan untuk bekerja dengan string, tetapi mereka memiliki tujuan dan hasil yang berbeda. Berikut adalah penjelasan tentang perbedaan keduanya:

* Gunakan `as_str()` ketika Anda ingin mendapatkan referensi ke string tanpa mengalokasikan memori baru. Ini berguna ketika Anda hanya perlu membaca string dan tidak perlu mengubahnya.

* Gunakan `into_owned()` ketika Anda ingin membuat salinan dari string slice (&str) dan mendapatkan String yang dimiliki. Ini berguna ketika Anda perlu menyimpan string dan memastikan bahwa Anda memiliki kepemilikan atas data tersebut.

Keduanya memiliki kegunaan masing-masing tergantung pada konteks di mana Anda bekerja dengan string dalam Rust.









## eof
