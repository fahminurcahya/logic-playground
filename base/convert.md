# Perbandingan Konversi dari Number ke String di Golang, TypeScript, Java, Dart, dan Rust

| **Bahasa**     | **Metode/Sintaks**          | **Contoh**                            | **Penjelasan**                                                  |
| -------------- | --------------------------- | ------------------------------------- | --------------------------------------------------------------- |
| **Golang**     | `strconv.Itoa(number)`      | `str := strconv.Itoa(123)`            | Menggunakan package `strconv` untuk mengubah integer ke string. |
|                | `fmt.Sprintf("%d", number)` | `str := fmt.Sprintf("%d", 123)`       | Menggunakan format string untuk konversi.                       |
| **TypeScript** | `number.toString()`         | `let str = (123).toString();`         | Memanggil metode `toString()` dari objek angka.                 |
|                | `` `${number}` ``           | `` let str = `${123}`; ``             | Menggunakan template literal untuk mengubah angka ke string.    |
| **Java**       | `String.valueOf(number)`    | `String str = String.valueOf(123);`   | Menggunakan metode `String.valueOf`.                            |
|                | `Integer.toString(number)`  | `String str = Integer.toString(123);` | Alternatif untuk tipe data `int`.                               |
| **Dart**       | `number.toString()`         | `String str = 123.toString();`        | Memanggil metode `toString()` bawaan.                           |
| **Rust**       | `number.to_string()`        | `let str = 123.to_string();`          | Memanggil metode `to_string()` bawaan pada tipe angka.          |
|                | `format!("{}", number)`     | `let str = format!("{}", 123);`       | Menggunakan makro format untuk konversi.                        |

## Penjelasan

1. **Golang**:

   - `strconv.Itoa`: Cara standar untuk mengubah integer ke string.
   - `fmt.Sprintf`: Berguna untuk format lebih kompleks atau angka desimal.

2. **TypeScript**:

   - `.toString()`: Cara standar untuk mengubah angka menjadi string.
   - Template literal: Praktis untuk menyisipkan angka ke dalam string.

3. **Java**:

   - `String.valueOf`: Cara universal untuk mengubah tipe data apapun ke string.
   - `Integer.toString`: Lebih spesifik untuk tipe data integer.

4. **Dart**:

   - `.toString()`: Cara langsung untuk mengubah angka menjadi string.

5. **Rust**:
   - `.to_string()`: Digunakan untuk semua tipe angka.
   - `format!`: Cocok untuk konversi sekaligus format output.
