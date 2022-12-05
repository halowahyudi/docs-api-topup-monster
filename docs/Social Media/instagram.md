---
sidebar_position: 2
---

# INSTAGRAM ✅

API ini mendapatkan Foto Profile dan Username jika terdaftar.

## HTTP GET

Endpoint: `https://api.topup.monster/check/instagram`

:::warning PENTING!!!
Jika Username Instagram tidak ditemukan maka responsenya bisa di validasi di HTTP Response, tidak berupa JSON. Kami berusaha menangani masalah ini.

:::

```php
<?php

$curl = curl_init();

curl_setopt_array($curl, array(
  CURLOPT_URL => 'https://api.topup.monster/check/instagram?username=xxx&api_key=xxx',
  CURLOPT_RETURNTRANSFER => true,
  CURLOPT_ENCODING => '',
  CURLOPT_MAXREDIRS => 10,
  CURLOPT_TIMEOUT => 0,
  CURLOPT_FOLLOWLOCATION => true,
  CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
  CURLOPT_CUSTOMREQUEST => 'GET',
));

$response = curl_exec($curl);

curl_close($curl);
echo $response;
```
