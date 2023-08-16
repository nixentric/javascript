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
