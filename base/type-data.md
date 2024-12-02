# Perbandingan Tipe Data Dasar di Golang, TypeScript, Java, Dart, dan Rust

| **Tipe Data**        | **Golang**                                    | **TypeScript**                   | **Java**                       | **Dart**                    | **Rust**                          | **Penjelasan**                                                      |
| -------------------- | --------------------------------------------- | -------------------------------- | ------------------------------ | --------------------------- | --------------------------------- | ------------------------------------------------------------------- |
| **Integer**          | `int`, `int8`, `int16`, `int32`, `int64`      | `number` (untuk integer & float) | `byte`, `short`, `int`, `long` | `int`                       | `i8`, `i16`, `i32`, `i64`, `i128` | Menyimpan bilangan bulat dengan ukuran berbeda.                     |
| **Unsigned Integer** | `uint`, `uint8`, `uint16`, `uint32`, `uint64` | _(Tidak Ada)_                    | _(Tidak Ada)_                  | _(Tidak Ada)_               | `u8`, `u16`, `u32`, `u64`, `u128` | Bilangan bulat tanpa tanda (hanya positif).                         |
| **Floating Point**   | `float32`, `float64`                          | `number`                         | `float`, `double`              | `double`                    | `f32`, `f64`                      | Menyimpan bilangan desimal atau pecahan.                            |
| **Boolean**          | `bool`                                        | `boolean`                        | `boolean`                      | `bool`                      | `bool`                            | Menyimpan nilai `true` atau `false`.                                |
| **Character**        | _(Tidak Ada)_                                 | _(Tidak Ada)_                    | `char`                         | `String` (untuk 1 karakter) | `char`                            | Menyimpan satu karakter Unicode.                                    |
| **String**           | `string`                                      | `string`                         | `String`                       | `String`                    | `String`                          | Menyimpan teks atau kumpulan karakter.                              |
| **Array**            | `[n]T` (array tetap)                          | `T[]`, `Array<T>`                | `T[]`                          | `List<T>`                   | `[T; n]` (array tetap)            | Menyimpan elemen tipe yang sama dalam jumlah tetap atau dinamis.    |
| **Slice/List**       | `[]T` (dinamis)                               | _(Gunakan Array)_                | `ArrayList<T>`                 | `List<T>`                   | `Vec<T>`                          | Struktur data dinamis untuk menyimpan elemen tipe yang sama.        |
| **Map/Dictionary**   | `map[K]V`                                     | `{ [key: K]: V }`                | `HashMap<K, V>`                | `Map<K, V>`                 | `HashMap<K, V>`                   | Pasangan kunci-nilai untuk pencarian cepat.                         |
| **Tuple**            | _(Tidak Ada)_                                 | `[T1, T2, ...]`                  | _(Tidak Ada)_                  | _(Tidak Ada)_               | `(T1, T2, ...)`                   | Menyimpan beberapa nilai dengan tipe berbeda dalam satu entitas.    |
| **Nil/Null**         | `nil`                                         | `null`, `undefined`              | `null`                         | `null`                      | `None` (dalam `Option`)           | Menyimpan nilai kosong atau tidak ada.                              |
| **Any**              | `interface{}`                                 | `any`                            | `Object`                       | `dynamic`                   | _(Tidak Ada)_                     | Menyimpan nilai dari tipe data apapun.                              |
| **Pointer**          | `*T`                                          | _(Tidak Ada)_                    | _(Tidak Ada)_                  | _(Tidak Ada)_               | `*const T`, `*mut T`              | Menyimpan referensi ke lokasi memori suatu variabel.                |
| **Enum**             | `const ( ... )`                               | `enum`                           | `enum`                         | `enum`                      | `enum`                            | Tipe data untuk kumpulan nilai konstan yang terdefinisi sebelumnya. |

## Penjelasan

1. **Integer**: Memiliki ukuran berbeda tergantung pada kebutuhan memori (8-bit hingga 128-bit).
2. **Floating Point**: Digunakan untuk menyimpan angka dengan nilai desimal.
3. **Boolean**: Menyimpan nilai `true` atau `false` untuk logika.
4. **String**: Digunakan untuk menyimpan teks, seperti nama atau kalimat.
5. **Array/Slice/List**: Struktur data untuk menyimpan banyak elemen bertipe sama.
6. **Map/Dictionary**: Menyimpan pasangan kunci dan nilai untuk pencarian yang cepat.
7. **Nil/Null**: Representasi nilai kosong atau tidak ada.
8. **Pointer**: Digunakan untuk manipulasi tingkat rendah pada memori (hanya tersedia di Golang dan Rust).
9. **Tuple**: Berguna untuk menyimpan beberapa nilai dengan tipe berbeda (tersedia di TypeScript dan Rust).
