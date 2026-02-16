# Pyhton Progress
## Apa Itu Python?

### Python adalah bahasa pemrograman paling populer (melampaui JavaScript di GitHub pada 2024) karena kesederhanaannya dan fleksibilitasnya di berbagai industri:

- Data Science & AI: Menjadi bahasa utama berkat pustaka seperti Pandas, NumPy, dan TensorFlow yang memudahkan analisis data serta pengembangan AI.

- Web Development: Memungkinkan pembuatan backend yang aman dan skalabel menggunakan framework seperti Django, FastAPI, dan Flask (digunakan oleh Instagram & Pinterest).

- Keamanan Siber: Digunakan oleh ahli cybersecurity untuk pemindaian otomatis dan analisis ancaman.

- IoT & Sistem Tertanam: Berjalan optimal di perangkat seperti Raspberry Pi untuk proyek smart home.

- Otomatisasi: Kekuatan utamanya ada pada efisiensi tugas repetitif, mulai dari olah spreadsheet hingga web scraping menggunakan Selenium dan BeautifulSoup.

Kesimpulan: Python adalah pilihan terbaik bagi pemula maupun profesional karena kemampuannya menangani proyek dari skala skrip sederhana hingga level industri.

# Untuk hari pertama kita akan belajar mengenai variable & tipe data

# Variable #

**Di Python, Anda cukup menulis nama variabel di sebelah kiri, diikuti oleh operator penugasan, dan nilai yang ingin Anda tetapkan ke variabel di sebelah kanan.**

Berikut contoh cara mendeklarasikannya. name & age variabel:

    name = 'John Doe'
    age = 25

**Dalam contoh di atas, variabel name memegang nilai 'John Doe'. Nilai ini adalah string, yaitu serangkaian karakter yang digunakan untuk merepresentasikan teks. String ditulis dengan tanda kutip tunggal (') atau ganda("), misalnya 'Hello' atau "Hello"**

Saat memberi nama variabel di Python, ada beberapa aturan penting yang harus Anda ingat:

  **Nama variabel hanya boleh diawali dengan huruf atau garis bawah ( _ ), bukan angka.**
  **Nama variabel hanya boleh berisi karakter alfanumerik ( a-z, A-Z, 0-9) dan garis bawah ( _ ).**
  **Nama variabel peka terhadap huruf besar dan kecil istilah ini disebut sensitive case — age, Age, Dan AGE semuanya dianggap unik.**
  **Nama variabel tidak boleh berupa salah satu kata kunci yang dicadangkan oleh Python, seperti if, class atau def.**

**Jika Anda melanggar salah satu aturan tersebut, program Python Anda akan menampilkan kesalahan.**

SyntaxError:

    5variable_name = 5
     ^
    SyntaxError: invalid syntax

Sekarang mari kita bahas beberapa konvensi penamaan umum untuk variabel di Python.

**Pertama, nama variabel harus ditulis dengan huruf kecil, dengan setiap kata dipisahkan oleh garis bawah. Ini disebut snake case:**

    my_variable_name = 'freeCodeCamp'

**Selanjutnya, Anda harus menggunakan nama yang deskriptif untuk variabel. Misalnya, jika Anda ingin menyimpan usia pengguna sebagai variabel, user_agelebih baik daripada ageatau singkatan seperti ua:**

    user_age = 30

Dengan cara ini, Anda dapat dengan mudah mengkomunikasikan tujuan suatu variabel kepada anggota tim lain (atau kepada diri Anda sendiri di masa depan) dalam basis kode yang besar.

**Konvensi lain adalah menghindari penggunaan nama variabel satu huruf. Ini sangat umum di Python, tetapi sebaiknya dihindari karena nama variabel dengan satu huruf tidak menyampaikan tujuan atau makna apa pun:**

    x = 56 # What do you mean by x?

**Ini berbeda jika Anda berada dalam sebuah perulangan atau sesuatu yang serupa, karena nama variabel seperti i, j, k, dan seterusnya adalah hal yang umum dan dapat diterima.**

**Anda dapat menggunakan komentar untuk menjelaskan kode Anda, meninggalkan pengingat untuk diri sendiri, atau mengklarifikasi mengapa suatu baris kode ada. Komentar sangat membantu terutama saat Anda belajar atau bekerja dalam tim.**

Namun, Anda tidak boleh menggunakan komentar untuk menjelaskan arti nama variabel Anda. Sebaliknya, nama yang Anda pilih untuk variabel Anda harus deskriptif dan mengkomunikasikan fungsinya, serta mengikuti aturan penamaan lain yang disebutkan sebelumnya untuk mencegah kesalahan sintaksis. 

# Tipe Data #

1. Bilangan bulat: Bilangan utuh tanpa desimal, misalnya, 10 atau -5.

        my_integer_var = 10
        print('Integer:', my_integer_var) # Integer: 10

2. Float: Angka dengan titik desimal, seperti 4.41 atau -0.4.

        my_float_var = 4.50
        print('Float:', my_float_var) # Float: 4.5

3. String: Serangkaian karakter yang diapit oleh tanda kutip tunggal atau ganda, seperti 'Hello world!'.

        my_string_var = 'hello'
        print('String:', my_string_var) # String: hello

4. Boolean: Tipe data benar atau salah, ditulis sebagai True atau False.

        my_boolean_var = True
        print('Boolean:', my_boolean_var) # Boolean: True

5. Himpunan: Kumpulan elemen unik yang tidak berurutan, seperti {4, 2, 0}.

        my_set_var = {7, 5, 8}
        print('Set:', my_set_var) # Set: {7, 5, 8}

6. Kamus: Kumpulan pasangan kunci-nilai yang diapit dalam tanda kurung kurawal, seperti {'name': 'John Doe', 'age': 28}.

        my_dictionary_var = {'name': 'Alice', 'age': 25}
        print('Dictionary:', my_dictionary_var) # Dictionary: {'name': 'Alice', 'age': 25}

7. Tuple: Koleksi terurut yang tidak dapat diubah, diapit dalam tanda kurung, seperti (7, 8, 4).

        my_tuple_var = (7, 5, 8)
        print('Tuple:', my_tuple_var) # Tuple: (7, 5, 8)

8. Rentang: Urutan angka, sering digunakan dalam perulangan, misalnya, range(5).

        my_range_var = range(5)
        print('Range:', my_range_var) # Range: range(0, 5)

9. Daftar: Kumpulan elemen yang terurut dan mendukung berbagai tipe data.

        my_list = [22, 'Hello world', 3.14, True]
        print(my_list) # [22, 'Hello world', 3.14, True]

10. Tidak ada: Nilai khusus yang mewakili ketiadaan suatu nilai.

        my_none_var = None
        print('None:', my_none_var) # None: None

**Untuk mendapatkan tipe data suatu variabel, Anda dapat menggunakan type() fungsi:**

        my_var_1 = 'Hello world'
        my_var_2 = 21

        print(type(my_var_1)) # <class 'str'>
        print(type (my_var_2)) # <class 'int'>

**Dan berikut adalah semua tipe data yang dibahas dalam pelajaran ini, beserta tipe datanya di terminal:**

        my_integer_var = 10
        print(type(my_integer_var))  # <class 'int'>

        my_float_var = 4.50
        print(type(my_float_var))  # <class 'float'>

        my_string_var = 'hello'
        print(type(my_string_var))  # <class 'str'>

        my_boolean_var = True
        print(type(my_boolean_var))  # <class 'bool'>

        my_set_var = {7, 5, 8}
        print(type(my_set_var))  # <class 'set'>

        my_dictionary_var = {'name': 'Alice', 'age': 25}
        print(type(my_dictionary_var))  # <class 'dict'>

        my_tuple_var = (7, 5, 8)
        print(type(my_tuple_var))  # <class 'tuple'>

        my_range_var = range(5)
        print(type(my_range_var))  # <class 'range'>

        my_list = [22, 'Hello world', 3.14, True]
        print(type(my_list)) # <class 'list'>

        my_none_var = None
        print(type(my_none_var))  # <class 'NoneType'>

**Terpasang isinstance(). Fungsi ini memungkinkan Anda untuk memeriksa apakah suatu variabel cocok dengan tipe data tertentu. Fungsi ini menerima sebuah objek dan tipe data yang ingin Anda periksa, kemudian mengembalikan nilai boolean. Berikut beberapa contohnya:**

        isinstance(isi data, tipe data) # Format
        
        isinstance('Hello world', str) # True
        isinstance(True, bool) # True
        isinstance(42, int) # True
        isinstance('John Doe', int) # False
