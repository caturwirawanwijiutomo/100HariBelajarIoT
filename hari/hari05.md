* protokol

Protokol untuk IoT dapat menggunakan protokol standar berbasis TCP/IP seperti HTTP namun pada prakteknya banyak juga yang menggunakan resource constrained protokol seperti CoAP dan MqTT. Persoalan pemilihan protokol dibasiskan pada stack yang didukung oleh perangkat IoT. di awal implementasinya banyak yang menggunakan perangkat gateway untuk menghubungkan perangkat yang tidak memiliki kapabilitas stack TCP/IP. 

perkembangan SoC pada perangkat IoT memungkinkan untuk TCP/IP diimplementasikan di software sehingga protokol yang digunakan untuk resource constrained protokol tidak menjadi persoalan lagi. dalam perkembangannya CoAP menjadi tidak populer karena tidak lebih baik dibandingkan dengan protokol REST melalui HTTP. MqTT masih menjadi protokol yang baik karena bersifat asinkron yang lebih sesuai dengan sifat resource constrained.
