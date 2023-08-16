# Hallo Dunia

Pada bagian ini kita akan mempelajari inti JavaScript.

## "script" Tag

Program JavaScript dapat disisipkan hampir di mana saja di dalam dokumen HTML dengan menggunakan tag ``<script>``.

Contohnya:

```html
<!DOCTYPE HTML>
<html>

<body>

  <p>Before the script...</p>

  <script>
    alert( 'Hello, world!' );
  </script>

  <p>...After the script.</p>

</body>

</html>
```
Di dalam tag ``<script>`` kita dapat menulis kode JavaScript. Dalam kasus ini, kode ``alert('Hello, world!');`` akan menampilkan kotak pesan (alert) dengan teks ``"Hello, world!"`` saat browser mengolah skrip tersebut.

## Markup Modern

``<script>`` memiliki beberapa atribut yang sudah jarang digunakan saat ini, tetapi masih bisa ditemui di kode-kode lama:

**Pertama, atribut ``type``: ``<script type=…>``**

Di masa lampau, saat stardar HTML masih menggunakan HTML4, atribut ``type`` masih wajib digunakan. Biasanya digunakan dalam bentuk seperti ini ``<script type="text/javascript">``. Tapi, saat ini, itu sudah tidak diperlukan lagi. Juga, di standar HTML modern, makna atribut ini juga telah berubah. Dan sekarang, atribut ``<type>`` digunakan saat kita ingin menggunakan JavaScript Modules (akan dibahas di lain kesempatan pada pembelajaran tingkat lanjut).

**Kedua, atribut ``language``: ``<script language=…>``**

Atribut ini digunakan untuk mendeklarasikan bahasa yang digunakan script. Atribut ini agak tidak masuk akal untuk digunakan karena JavaScript merupakan bahasa bawaan dari tag ``<script>``. Jadi, atribut ini tidak perlu dipakai.

**Skrip Pembuka & Penutup Komentar (Comment)**

Di dalam buku dan panduan jadul, kamu mungkin sering menemukan skrip comment di dalam ``<script>``, seperti ini:

```html
<script type="text/javascript"><!--
    ...
//--></script>
```
Pada JavaScript modern, trik ini sudah tidak digunakan lagi. Awalnya trik ini digunakan untuk menyembunyikan kode JavaScript dari peramban (browser) yang sudah sangat tua dan tidak memiliki pemahaman tentang cara memproses tag ``<script>``. Di masa lalu, beberapa peramban mungkin tidak sepenuhnya memahami atau mendukung tag ``<script>``, dan ini bisa menyebabkan masalah dalam menjalankan kode JavaScript di dalamnya.

Dengan menggunakan komentar seperti ``<!--`` dan ``-->``, tujuan awalnya adalah membuat kode JavaScript tetap tidak terlihat oleh peramban-peramban tua tersebut. Kode JavaScript akan diapit oleh komentar ini sehingga peramban yang tidak tahu bagaimana memproses tag ``<script>`` akan mengabaikan kode di dalamnya.

Namun, pada peramban modern yang telah dirilis dalam 15 tahun terakhir, masalah ini sudah tidak ada lagi. Peramban modern mampu memahami tag ``<script>`` dengan baik, dan kode JavaScript di dalamnya akan dieksekusi tanpa masalah. Karena itu, trik komentar semacam ini tidak diperlukan lagi dalam JavaScript modern.


