Nama    : Ikomang Alit Arianta
NIM     : 230010055

1. Direktori konfigurasi
database.php: Ini adalah file yang penting untuk mengonfigurasi basis data. Menggunakan PHP Data Objects (PDO), file ini menetapkan parameter kunci seperti host, nama basis data, pengguna, dan sandi. Dibuat untuk mengelola koneksi basis data dengan aman, file ini juga memiliki penanganan pengecualian untuk mengatasi dan menyelesaikan masalah koneksi.

2. Direktori publik
index.php: Sebagai gerbang masuk aplikasi, file ini adalah yang pertama kali diakses oleh pengunjung situs. Saat ini, file ini hanya menampilkan judul "Titik Akses API XYZ Sales", menandakan titik akses API untuk aplikasi penjualan XYZ.

3. Direktori sumber
3.1. Sub-direktori Pengendali
CustomerController.php: Menangani operasi CRUD untuk data pelanggan. File ini menyediakan metode untuk mengakses, menambah, memperbarui, dan menghapus informasi pelanggan, berkolaborasi dengan model Customers.php.
PurchaseController.php: Bertugas mengelola operasi CRUD untuk transaksi pembelian. File ini memfasilitasi pengambilan dan manipulasi data pembelian, berkerja sama dengan model Purchases.php.
SalesController.php: Mengurus operasi CRUD untuk data penjualan. File ini memungkinkan pengambilan dan perubahan informasi penjualan, berinteraksi dengan model Sales.php.
Semua pengendali ini dirancang untuk menanggapi dan memproses permintaan HTTP sesuai dengan fungsi yang ditentukan.

3.2. Sub-direktori Model
Customers.php: Bertanggung jawab atas eksekusi query terkait data pelanggan, berdasarkan instruksi dari CustomerController.php, dan menjembatani aplikasi dengan basis data pelanggan.
Purchases.php: Melaksanakan query untuk data pembelian, menerima instruksi dari PurchaseController.php, dan memastikan koneksi yang stabil dengan basis data pembelian.
Sales.php: Menjalankan query yang terkait dengan data penjualan, sesuai dengan perintah dari SalesController.php, dan memelihara integrasi dengan basis data penjualan.
Setiap model ini menerapkan serangkaian query untuk mengambil, memasukkan, memperbarui, dan menghapus data, memastikan aplikasi dapat berinteraksi dengan basis data secara efisien dan efektif.

Tantangan yang Terhadap
Salah satu rintangan utama adalah mengimplementasikan operasi CRUD dengan efektif. Mengkoordinasikan antara Pengendali dan Model untuk memastikan pemrosesan data yang tepat merupakan tugas yang rumit dan membutuhkan pemahaman yang mendalam tentang arsitektur MVC.

Ini merupakan sesuatu yang baru bagi saya, dan awalnya, saya merasa terbebani. Saya juga menghadapi kesulitan dalam mengelola ketergantungan antara kelas-kelas dan memastikan koneksi basis data berjalan dengan baik sangat penting. Saya harus menjamin setiap model dapat berinteraksi dengan basis data dengan efisien.

Mengatasi Tantangan
Untuk menanggulangi tantangan CRUD ini, saya menginvestasikan waktu untuk menyelami dokumentasi PHP dan MySQL secara teliti, sambil mencari tambahan sumber daya seperti tutorial dan forum komunitas. Pendekatan ini memungkinkan saya untuk menyelesaikan bug dan meningkatkan efisiensi kode.

Saya juga memanfaatkan sumber daya pembelajaran seperti tutorial YouTube, yang membuktikan sangat berguna dalam memberikan arahan dan pengetahuan yang diperlukan.