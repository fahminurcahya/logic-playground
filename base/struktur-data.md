# Perbandingan Struktur Data di Golang, TypeScript, Java, Dart, dan Rust

| **Struktur Data**  | **Golang**                   | **TypeScript**                        | **Java**                                      | **Dart**                           | **Rust**                             | **Kegunaan**                                                               |
| ------------------ | ---------------------------- | ------------------------------------- | --------------------------------------------- | ---------------------------------- | ------------------------------------ | -------------------------------------------------------------------------- |
| **Array**          | `[5]int{1, 2, 3, 4, 5}`      | `let arr: number[] = [1, 2, 3, 4, 5]` | `int[] arr = {1, 2, 3, 4, 5};`                | `List<int> arr = [1, 2, 3, 4, 5];` | `[1, 2, 3, 4, 5]` (Fixed Size)       | Menyimpan elemen dengan jumlah tetap dan tipe data yang sama.              |
| **Slice**          | `[]int{1, 2, 3, 4, 5}`       | _(Tidak Ada, gunakan Array)_          | _(Tidak Ada, gunakan List/ArrayList)_         | _(Tidak Ada, gunakan List)_        | `vec![1, 2, 3, 4, 5]` (Dynamic Size) | Versi dinamis dari array, memungkinkan penambahan atau penghapusan elemen. |
| **Map/Dictionary** | `map[string]int{"a": 1}`     | `let map: { [key: string]: number }`  | `Map<String, Integer> map = new HashMap<>();` | `Map<String, int> map = {'a': 1};` | `HashMap<String, i32>::new()`        | Menyimpan pasangan kunci-nilai untuk pencarian data dengan kunci unik.     |
| **Struct/Object**  | `type Person struct {...}`   | `interface Person {...}`              | `class Person {...}`                          | `class Person {...}`               | `struct Person {...}`                | Digunakan untuk merepresentasikan entitas dengan atribut dan perilaku.     |
| **List**           | _(Tidak Ada, gunakan Slice)_ | `let list: Array<number> = [1, 2, 3]` | `List<Integer> list = new ArrayList<>();`     | `List<int> list = [1, 2, 3];`      | `Vec<i32>::new()`                    | Menyimpan elemen secara dinamis dengan ukuran fleksibel.                   |
| **Set**            | _(Tidak Ada, gunakan Map)_   | _(Gunakan Array/List)_                | `Set<Integer> set = new HashSet<>();`         | `Set<int> set = {1, 2, 3};`        | `HashSet::new()`                     | Menyimpan elemen unik tanpa duplikasi.                                     |
| **Queue**          | _(Implementasi manual)_      | _(Gunakan Array/List)_                | `Queue<Integer> queue = new LinkedList<>();`  | `Queue<int> queue = Queue();`      | _(Implementasi manual)_              | Struktur data FIFO (First-In-First-Out) untuk antrian tugas/data.          |
| **Stack**          | _(Implementasi manual)_      | _(Gunakan Array/List)_                | `Stack<Integer> stack = new Stack<>();`       | _(Tidak Ada, gunakan List/Queue)_  | `VecDeque::new()`                    | Struktur data LIFO (Last-In-First-Out) untuk menyimpan data sementara.     |

## Penjelasan Kegunaan

1. **Array**: Digunakan ketika ukuran data tetap dan sudah diketahui sebelumnya.
2. **Slice/List**: Cocok untuk data dengan ukuran yang dapat berubah, memungkinkan penambahan atau penghapusan elemen secara dinamis.
3. **Map/Dictionary**: Berguna untuk pencarian cepat berdasarkan kunci, seperti untuk menyimpan konfigurasi, nilai unik, atau pemetaan data.
4. **Struct/Object**: Digunakan untuk merepresentasikan entitas atau objek dengan atribut dan perilaku tertentu.
5. **Set**: Memastikan bahwa elemen dalam koleksi tetap unik dan tidak ada duplikasi.
6. **Queue**: Digunakan untuk kasus di mana elemen harus diproses dalam urutan yang tepat, yaitu elemen pertama yang masuk adalah yang pertama keluar (FIFO).
7. **Stack**: Menyimpan elemen dalam urutan LIFO, berguna dalam algoritma rekursi atau operasi undo/redo.
