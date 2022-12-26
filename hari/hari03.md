## hardware platform

Untuk membangun IoT kita akan memulai dari edge yaitu endpoint dari arsitektur IoT dalam hal ini adalah hardware node atau disebut juga sebagai edge. hardware ini perlu untuk memiliki kapabilitas koneksi dan selanjutnya bertindak menjadi sensor/aktuator.

### Proprietary

Jika kita datang dari dunia otomasi dan manufaktur, platform hardware yg digunakan adalah PLC. PLC memiliki standar menggunakan ladder logic. bahasa ini memiliki keunggulan karena jelas terstruktur dan to the point. walaupun untuk persoalan koneksi ke internet biasanya PLC memerlukan modul tambahan. 

modul ini cukup mahal dan memerlukan setting vendor untuk dapat terhubung menggunakan stack TCP/IP.

### Open source

Sebelum kita membahas dua platform open source yaitu 
- arduino (berbasis microcontroller, RTOS)
- Raspberry pi (berbasis mikroprosesor, General purpose OS capable)

kita perlu membahas terlebih dahulu bagaimana keadaan dunia sebelum ada dua solusi ini. perlu diketahui membangun hardware dari awal bukan perkara gampang, apalagi hardware development sebelum ada open source. terkadang kita perlu membeli lisensi untuk sekedar bisa memasukkan program ke platform yg kita pilih. contohnya di dunia automasi menggunakan PLC semua tools berbayar dan hanya digunakan spesifik untuk merk tertentu.

namun beberapa vendor mulai menggunakan opens source, berawal dari toolchain yang dibangun berbasis GNU yg open source. karena itu atmel yg sekarang dibeli oleh microchip adalah salah satu vendor microcontroller yg melakukan itu dan itu menjadi jalan dari arduino untuk muncul dengan meng-extend library dan compiler atmel ke tools yg jauh lebih sederhana bisa diakses pemula.

Untuk mikroprosesor jauh lebih sulit karena awalnya kita perlu membeli OS khusus yg berjalan di atas microprocessor embedded system. hal ini membutuhkan investasi awal yg tidak sedikit. Linux yg open source mengubah ini semua, Linux memungkinkan setiap orang untuk membangun OS sendiri di mikroprosesor apa pun, walaupun awalnya ini sulit karena beberapa mikroprosesor unik dan diperlukan perjanjian NDA untuk mengtahui perintah (microcode) dan register mendevelop OS untuk mikroprosesor tertentu sehingga terkadang developer OS menebak-nebak. hal ini berlangsung cukup lama, walaupun tidak menyurutkan semangat untuk mengimplementasi di Linux.

hal ini berubah sejak raspberry pi muncul, penemu nya merupakan karyawan broadcom salah satu vendor mikroprosesor, dia mengusulkan dan memberikan proposal ke tempat ia bekerja untuk melepas satu jenis mikroporsseo yg awalnya digunakan untuk set top box tv untuk dapat digunakan untuk PC kecil yg murah dan dapat dibeli semua orang, walaupun pada awalnya tidak mulus karena beberapa komponen berupa binary tapi kesuksesan raspberry pi dan menjadi platform dengan penjualan terbesar justru mendapat dukungan dari broadcom dan mengembangkan prosessor ini untuk versi raspberry pi yg jauh lebih baik. saat artikel ini ditulis versi raspberryp i adalh versi 4 dengan 1.5 Ghz dan memori hingga 8 GB. 

Kesuksesan arduino dan raspberry pi membuat vendor mikroprosesor untuk memasarkan produknya dalam open source bahkan membuka dokumentasi mereka secara lengkap. salah satu yg mengikuti kesuksesan adalah ESP886 dan ESP32 dan ada pula pabrikan rockwell chip juga mengembangkan platform mirip raspberry pi dengan variasi tertentu. 

Platform open source jelas mengubah perspektif orang, tidak ada masa dimana anda bisa dengan mudah membangun hardware IoT anda sendiri berbasis platform ini, perlahan namun pasti platform open source ini mulai masuk ke industri yg menjadi kekhususan solusi PLC/proprietary dengan diluncurkannya arduino untuk industri dan mendukung pemrograman PLC dan raspberry pi yg membuat compute module untuk selanjutnya memungkinkan orang memgenbangkan board sendiri untuk kebutuhan yang spesifik bahkan untuk militer. 




