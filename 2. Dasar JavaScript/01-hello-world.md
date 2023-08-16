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
