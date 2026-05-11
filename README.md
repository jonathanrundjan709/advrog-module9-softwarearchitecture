# Tutorial 8

## a. What is AMQP?

AMQP adalah singkatan dari Advanced Message Queuing Protocol. AMQP merupakan protokol komunikasi untuk pertukaran pesan antar aplikasi melalui message broker, misalnya RabbitMQ.

Dengan AMQP, aplikasi publisher dapat mengirim pesan ke broker, lalu aplikasi subscriber atau consumer dapat menerima pesan tersebut. Pola ini membuat komunikasi antar aplikasi menjadi asynchronous, sehingga pengirim pesan tidak harus menunggu penerima memproses pesan secara langsung.

## b. What does `guest:guest@localhost:5672` mean?

Bagian `guest:guest@localhost:5672` adalah informasi koneksi ke server AMQP.

- `guest` pertama adalah username yang digunakan untuk login ke broker.
- `guest` kedua adalah password dari username tersebut.
- `localhost` berarti server broker berjalan di komputer lokal.
- `5672` adalah port default yang digunakan oleh AMQP, khususnya RabbitMQ, untuk menerima koneksi dari aplikasi.

Jadi, `guest:guest@localhost:5672` berarti aplikasi mencoba terhubung ke broker AMQP di komputer sendiri melalui port `5672`, menggunakan username `guest` dan password `guest`.
