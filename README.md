# Knutt-Morris-Pratt String Matching Algorithm

Knutt-Morris-Pratt adalah salah satu algoritma string matching yang digunakan untuk pencarian pola dalam suatu string.

## Cara Penggunaan

```php
<?php
require_once 'kmp.php';

$text = "abcabaabcabac";
$pattern = "abaa";

$result = kmp($text, $pattern);
if ($result === false)
{
  echo "Tidak ditemukan";
}
else
{
  echo "Ditemukan pada index ke " . $result;
}

```

## Dokumentasi
### kmp(<i>$text, $pattern</i>);
| Parameter | Tipe Data | Deskripsi |
| --------- | --------- | --------- |
| <b>$text</b> | string | String yang akan dilakukan pencarian menggunakan pola tertentu |
| <b>$pattern</b> | string | Pola yang digunakan untuk pencarian |

<i><b>return: index(int), false jika gagal</b></i>
