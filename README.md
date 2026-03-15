<<<<<<< HEAD
# new_flutter_tugasui

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Learn Flutter](https://docs.flutter.dev/get-started/learn-flutter)
- [Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Flutter learning resources](https://docs.flutter.dev/reference/learning-resources)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
=======
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



>>>>>>> 26ba017be6b131a994d8a0ac216e8a990a1d7a13
