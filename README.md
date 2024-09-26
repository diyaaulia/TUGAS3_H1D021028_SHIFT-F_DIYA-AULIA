1. Struktur Proyek
Struktur proyek kita terdiri dari beberapa file utama dalam folder lib/:

main.dart: Titik masuk aplikasi.
login.dart: Layar untuk login pengguna.
home.dart: Layar beranda setelah login.
2. pubspec.yaml
Di sini kita menambahkan dependensi shared_preferences, yang memungkinkan kita untuk menyimpan data lokal di perangkat pengguna.
3. membuat main.dart
main(): Fungsi utama yang menjalankan aplikasi.
MyApp: Widget utama yang mengatur material app dan rute.
initialRoute: Menentukan rute awal, di sini adalah LoginScreen.
routes: Mendefinisikan rute yang tersedia dalam aplikasi.
4. Membuat login.dart
TextEditingController: Mengontrol input dari TextField.
_login: Fungsi untuk menyimpan username dan mengalihkan pengguna ke layar beranda.
Menggunakan SharedPreferences untuk menyimpan data secara lokal.
Navigator.pushReplacementNamed: Mengalihkan pengguna ke /home setelah login berhasil.
build: Mengatur tampilan layar login dengan TextField dan tombol login.
5. Home.dart
HomeScreen: Widget beranda yang akan ditampilkan setelah login.
initState: Dipanggil saat widget pertama kali dimuat. Kita memanggil _loadUsername untuk mengambil username yang disimpan.
_loadUsername: Mengambil data username dari SharedPreferences dan memperbarui tampilan.

Login: Mengambil input dari pengguna dan menyimpannya.
Routing: Memungkinkan navigasi antar layar.
Local Storage: Menyimpan username dengan menggunakan shared_preferences.
Side Menu: Memfasilitasi logout dan navigasi lainnya.Login: Mengambil input dari pengguna dan menyimpannya.
Routing: Memungkinkan navigasi antar layar.
Local Storage: Menyimpan username dengan menggunakan shared_preferences.
Side Menu: Memfasilitasi logout dan navigasi lainnya.
