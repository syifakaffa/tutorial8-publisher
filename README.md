## Tutorial 8
Nama: Syifa Kaffa Billah

NPM: 2206816430

Kelas: C

**1. How many data your publisher program will send to the message broker in one run?**

Dalam program publisher yang telah dibuat, fungsi `main` menginisialisasi sebuah publisher p untuk message broker
`CrosstownBus`, kemudian mempublish lima event `UserCreatedEventMessage` menggunakan metode publish_event dari publisher
tersebut. Oleh karena itu, dalam satu jalannya program, **publisher mengirimkan lima pesan data ke message broker**.


**2. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?**

URL "amqp://guest:guest@localhost:5672" biasanya digunakan untuk terhubung ke message broker menggunakan AMQP.
Jika URL yang digunakan dalam program publisher dan program subscriber keduanya sama, ini berarti bahwa kedua
program terhubung ke instansi message broker yang sama yang berjalan pada mesin yang sama, menggunakan kredensial
otentikasi dan nomor port yang sama juga. Hal tersebut ditujukan untuk memastikan bahwa publisher dapat menpublish pesan
ke instansi message broker yang sama di mana subscriber berlangganan.