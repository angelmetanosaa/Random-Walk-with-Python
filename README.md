# Random-Walk-with-Python
Proses penyebaran suatu penyakit/virus dapat disimulasikan secara sederhana dengan menggunakan Random Walk. Pada metode ini, setiap individu direpresentasikan sebagai partikel yang bergerak bebas secara acak. Proses simulasi diawali dengan mendefinisikan sejumlah individu dari suatu komunitas yang sudah terinfeksi. Setelah itu, simulasi dilakukan dengan mendefinisikan perubahan posisi dari masing-masing individu secara acak. Secara sederhana, proses infeksi terjadi pada saat individu sehat berada pada posisi yang sama dengan individu yang terinfeksi. Selain itu, individu yang sudah sembuh diasumsikan memiliki imun terhadap penyakit/virus sehingga tidak akan terinfeksi untuk kedua kalinya. Proses simulasi berakhir setelah tidak ada lagi individu yang terinfeksi.

Algoritma: Penyebaran penyakit/virus dengan Random Walk
1. Inisialisasi variabel scalar
- jumlah individu
- rasio individu yang terinfeksi
- waktu pemulihan
- ukuran ruang simulasi
- probabilitas individu bergerak

2. Inisialisasi variabel list
- posisi masing-masing individu
- status kesehatan individu (individu dengan rasio tertentu berstatus terinfeksi)
- status imunitas individu
- waktu terinfeksi individu

Iterasi
Selama jumlah individu terinfeksi > 0:
- Untuk setiap individu:
- Update posisi berdasarkan probabilitas individu bergerak
- Koreksi posisi dengan PBC
- Update waktu terinfeksi untuk individu yang sudah terinfeksi.
- Update status kesehatan individu - recovery
- Jika waktu terinfeksi > waktu pemulihan, maka individu yang terinfeksi didefinisikan pulih
- Update status imun individu (individu yang sudah pulih memiliki imun sehingga tidak akan terinfeksi lagi)
- Update status kesehatan individu – infection
- Hitung jarak individu sehat dengan individu terinfeksi
- Jika jarak individu sehat dengan individu terinfeksi adalah nol, dan individu sehat tersebut belum memiliki imun, maka individu sehat tersebut akan terinfeksi
- Hitung dan simpan jumlah individu terinfeksi

Buatlah simulasi penyebaran penyakit/virus dengan menggunakan Random Walk 4
Arah dengan menggunakan variabel-variabel berikut:
1. Jumlah individu: 200
2. Rasio individu terinfeksi: 5%
3. Probabilitas individu bergerak: 80%
4. Waktu pemulihan: 10 hari
5.  Ukuran ruang simulasi: 20 x 20 unit
6. Lakukan simulasi dan buatlah plot jumlah individu yang terinfeksi tiap harinya.
7. Tentukan waktu pemulihan yang diperlukan oleh komunitas tersebut.
