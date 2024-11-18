# LAPORAN HASIL PENGERJAAN WEATHER

### Nama : Arif Prasojo
### Kelas / No. Absen : SIB 3E / 07
### Nim : 2241760100

<img src=image.png>

#### Penjelasan

Ketika aplikasi dijalankan, langkah pertama yang dilakukan adalah menentukan lokasi pengguna secara otomatis. Proses ini memanfaatkan fitur **GPS** (Global Positioning System) yang ada pada perangkat pengguna untuk mendapatkan koordinat geografis berupa **latitude** dan **longitude**. Informasi lokasi ini sangat penting karena menjadi dasar untuk mengambil data cuaca yang akurat dan relevan sesuai dengan posisi pengguna saat ini.

Setelah koordinat lokasi ditemukan, aplikasi akan mengirimkan permintaan ke layanan **API OpenWeather** untuk mengambil data cuaca terbaru berdasarkan informasi koordinat tersebut. Proses pengambilan data ini dilakukan secara otomatis di latar belakang untuk memastikan pengalaman pengguna yang mulus. Data cuaca yang diambil meliputi beberapa informasi penting, antara lain:

1. **Suhu Udara**: Ditampilkan dalam satuan **derajat Celcius** agar mudah dipahami oleh pengguna di wilayah yang menggunakan sistem metrik.
2. **Tekanan Udara**: Diukur dalam satuan **hPa (hectopascal)**, memberikan gambaran tentang kondisi atmosfer di lokasi pengguna.
3. **Kelembapan Udara**: Dinyatakan dalam bentuk persentase (%), menunjukkan jumlah uap air yang terkandung di udara.
4. **Tingkat Tutupan Awan**: Juga dinyatakan dalam bentuk persentase (%), memberikan indikasi seberapa banyak langit yang tertutup oleh awan.
5. **Nama Kota**: Nama kota atau wilayah yang sesuai dengan koordinat lokasi pengguna untuk memastikan bahwa data cuaca yang ditampilkan relevan dengan posisi mereka.

Saat data cuaca berhasil diterima dari API, aplikasi akan memproses dan memperbarui tampilan antarmuka pengguna (UI) untuk menampilkan informasi tersebut secara jelas dan menarik. Proses pembaruan ini dirancang agar terjadi secara real-time, sehingga pengguna dapat langsung melihat kondisi cuaca terkini tanpa perlu melakukan pembaruan manual.

Namun, sebelum data berhasil dimuat, aplikasi akan menampilkan indikator **loading** berupa animasi lingkaran yang berputar. Hal ini memberikan isyarat visual kepada pengguna bahwa aplikasi sedang bekerja untuk memuat data. Indikator loading memastikan pengguna tidak merasa aplikasi sedang macet atau mengalami gangguan, melainkan memberi tahu bahwa proses sedang berlangsung.

Selain memberikan data cuaca berdasarkan lokasi pengguna, aplikasi ini juga memungkinkan pengguna untuk mencari informasi cuaca di lokasi lain dengan mengetikkan nama kota yang mereka inginkan. Setelah nama kota dimasukkan, aplikasi akan mengirimkan permintaan ke API OpenWeather untuk mengambil data cuaca dari kota tersebut dan menampilkan hasilnya dengan format yang sama.

Fungsi utama aplikasi ini adalah memberikan kemudahan kepada pengguna dalam mengetahui kondisi cuaca terkini, baik di lokasi mereka maupun di tempat lain yang mereka minati. Dengan desain yang sederhana dan intuitif, aplikasi ini cocok digunakan untuk berbagai kebutuhan, seperti merencanakan perjalanan, memutuskan pakaian yang akan dikenakan, atau hanya sekadar mengetahui kondisi lingkungan sekitar. Kombinasi penggunaan teknologi GPS, API OpenWeather, dan indikator loading memastikan aplikasi ini dapat memberikan pengalaman yang andal, cepat, dan mudah digunakan.