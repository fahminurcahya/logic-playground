# Perbandingan Ternary Operation di Golang, TypeScript, Java, Dart, dan Rust

| **Bahasa**     | **Sintaks**                             | **Contoh**                                         | **Penjelasan**                                                                 |
| -------------- | --------------------------------------- | -------------------------------------------------- | ------------------------------------------------------------------------------ |
| **Golang**     | _(Tidak Ada)_                           | `result := if condition { a } else { b }`          | Golang tidak mendukung operator ternary. Gunakan ekspresi `if-else` sederhana. |
| **TypeScript** | `condition ? expr1 : expr2`             | `let result = isTrue ? "Yes" : "No";`              | Jika `isTrue` bernilai `true`, hasilnya adalah `"Yes"`, jika `false`, `"No"`.  |
| **Java**       | `condition ? expr1 : expr2`             | `String result = isTrue ? "Yes" : "No";`           | Sama seperti TypeScript, mendukung ternary untuk ekspresi sederhana.           |
| **Dart**       | `condition ? expr1 : expr2`             | `var result = isTrue ? "Yes" : "No";`              | Sama seperti TypeScript, digunakan untuk memilih nilai berdasarkan kondisi.    |
| **Rust**       | `if condition { expr1 } else { expr2 }` | `let result = if is_true { "Yes" } else { "No" };` | Tidak memiliki operator ternary langsung, tetapi mendukung ekspresi `if-else`. |

## Penjelasan Ternary Operation

1. **Sintaks Dasar**: Operator ternary memungkinkan Anda memilih antara dua nilai berdasarkan kondisi boolean. Sintaks umumnya adalah `condition ? expr1 : expr2`.
2. **Bahasa tanpa Ternary**: Golang dan Rust tidak memiliki operator ternary secara langsung, tetapi mendukung ekspresi `if-else` yang sederhana dan fungsional.
3. **Penggunaan Umum**:
   - Untuk memilih nilai berdasarkan kondisi, misalnya:
     ```dart
     // Dart
     var ageGroup = age > 18 ? "Adult" : "Minor";
     ```
   - Dalam inisialisasi atau parameter fungsi:
     ```typescript
     // TypeScript
     console.log(isValid ? "Valid" : "Invalid");
     ```
