# Perbandingan String Manipulation di Golang, TypeScript, Java, Dart, dan Rust

| **Operasi**              | **Golang**                               | **TypeScript**              | **Java**                          | **Dart**                       | **Rust**                    | **Kegunaan**                                          |
| ------------------------ | ---------------------------------------- | --------------------------- | --------------------------------- | ------------------------------ | --------------------------- | ----------------------------------------------------- |
| **Concatenation**        | `str1 + str2`                            | `str1 + str2`               | `str1 + str2`                     | `str1 + str2`                  | `str1.to_string() + str2`   | Menggabungkan dua atau lebih string.                  |
| **Substring**            | `str[start:end]`                         | `str.slice(start, end)`     | `str.substring(start, end)`       | `str.substring(start, end)`    | `str[start..end]`           | Mengambil bagian tertentu dari string.                |
| **Find/Substring Index** | `strings.Index(str, "substring")`        | `str.indexOf("substring")`  | `str.indexOf("substring")`        | `str.indexOf("substring")`     | `str.find("substring")`     | Mencari indeks pertama kemunculan substring.          |
| **Replace**              | `strings.Replace(str, "old", "new", -1)` | `str.replace("old", "new")` | `str.replace("old", "new")`       | `str.replaceAll("old", "new")` | `str.replace("old", "new")` | Mengganti kemunculan substring dengan yang baru.      |
| **Trim**                 | `strings.TrimSpace(str)`                 | `str.trim()`                | `str.trim()`                      | `str.trim()`                   | `str.trim()`                | Menghapus spasi di awal dan akhir string.             |
| **Split**                | `strings.Split(str, ",")`                | `str.split(",")`            | `str.split(",")`                  | `str.split(",")`               | `str.split(",")`            | Memecah string menjadi array berdasarkan delimiter.   |
| **To Lower Case**        | `strings.ToLower(str)`                   | `str.toLowerCase()`         | `str.toLowerCase()`               | `str.toLowerCase()`            | `str.to_lowercase()`        | Mengubah string menjadi huruf kecil.                  |
| **To Upper Case**        | `strings.ToUpper(str)`                   | `str.toUpperCase()`         | `str.toUpperCase()`               | `str.toUpperCase()`            | `str.to_uppercase()`        | Mengubah string menjadi huruf besar.                  |
| **Check Empty**          | `len(str) == 0`                          | `str.length === 0`          | `str.isEmpty()`                   | `str.isEmpty()`                | `str.is_empty()`            | Mengecek apakah string kosong.                        |
| **Join**                 | `strings.Join([]string{"a", "b"}, ",")`  | `arr.join(",")`             | `String.join(",", arr)`           | `arr.join(",")`                | `arr.join(",")`             | Menggabungkan array string menjadi satu string.       |
| **Length**               | `len(str)`                               | `str.length`                | `str.length()`                    | `str.length`                   | `str.len()`                 | Mendapatkan panjang string.                           |
| **Contains**             | `strings.Contains(str, "substring")`     | `str.includes("substring")` | `str.contains("substring")`       | `str.contains("substring")`    | `str.contains("substring")` | Mengecek apakah string mengandung substring tertentu. |
| **Format**               | `fmt.Sprintf("Hello %s", name)`          | `\`Hello ${name}\``         | `String.format("Hello {}", name)` | `"Hello ${name}"`              | `format!("Hello {}", name)` | Membuat string dengan format tertentu.                |

## Penjelasan Kegunaan

1. **Concatenation**: Digunakan untuk menggabungkan dua atau lebih string.
2. **Substring**: Untuk mengambil bagian tertentu dari string, misalnya substring pertama atau bagian tengah.
3. **Find/Substring Index**: Menemukan posisi pertama kemunculan substring dalam string.
4. **Replace**: Mengganti semua kemunculan substring dengan string yang baru.
5. **Trim**: Menghapus karakter spasi atau whitespace di awal dan akhir string.
6. **Split**: Memecah string menjadi array atau daftar berdasarkan delimiter tertentu.
7. **To Lower/Upper Case**: Mengubah semua huruf dalam string menjadi huruf kecil atau besar.
8. **Check Empty**: Mengecek apakah string kosong atau tidak.
9. **Join**: Menggabungkan array atau list string menjadi satu string dengan delimiter.
10. **Length**: Menghitung jumlah karakter dalam string.
11. **Contains**: Mengecek apakah string mengandung substring tertentu.
12. **Format**: Membuat string dengan format tertentu, berguna dalam pencetakan nilai dinamis dalam string.
