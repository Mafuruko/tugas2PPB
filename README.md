# Muhammad Naufal Dzakwan  
## NRP: 5025231234  


## Tugas 2 - Widget & State

## Deskripsi
Project ini merupakan tugas Flutter sederhana untuk mempraktikkan penggunaan **widget** dan **state** dalam pembuatan antarmuka aplikasi.

Aplikasi menampilkan:
- **AppBar** dengan judul aplikasi
- **Gambar** yang ditampilkan dari folder assets
- **Teks deskripsi**
- **Menu kategori** dengan ikon
- **Counter** yang dapat bertambah saat tombol `+` ditekan

Project ini menggunakan:
- `StatelessWidget`
- `StatefulWidget`
- `Container`
- `Column`
- `Row`
- `Padding`
- `SizedBox`
- `Image.asset`
- `ElevatedButton`
- `setState()`

---

## Tampilan Fitur
Fitur utama yang ada pada aplikasi ini:

1. **AppBar**
   - Menampilkan judul **My First App**

2. **Image Section**
   - Menampilkan gambar dari folder `assets`

3. **Text Section**
   - Menampilkan teks:  
     `What image is that`

4. **Category Section**
   - Menampilkan 3 kategori:
     - Food
     - Scenery
     - People

5. **Counter Section**
   - Menampilkan nilai counter
   - Tombol `+` digunakan untuk menambah nilai counter menggunakan `setState()`

---

## Struktur Widget
Struktur utama aplikasi:

- `MaterialApp`
- `Scaffold`
  - `AppBar`
  - `SingleChildScrollView`
    - `Padding`
      - `Column`
        - `Container` gambar
        - `Container` teks
        - `Container` kategori
        - `Container` counter

---

## Penjelasan State
Aplikasi ini menggunakan `StatefulWidget` pada `HomePage` karena terdapat data yang dapat berubah, yaitu nilai counter.

```dart
int counter = 4;
````

Saat tombol `+` ditekan, nilai counter akan bertambah:

```dart
setState(() {
  counter++;
});
```

`setState()` digunakan agar tampilan aplikasi diperbarui secara otomatis setiap kali nilai counter berubah.

---

## Asset

Pastikan gambar disimpan pada folder berikut:

```bash
assets/img.jpg
```

Lalu daftarkan asset di file `pubspec.yaml`:

```yaml
flutter:
  uses-material-design: true
  assets:
    - assets/img.jpg
```

## Screenshot




