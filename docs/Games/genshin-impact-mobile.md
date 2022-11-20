---
sidebar_position: 2
---

# Genshin Impact Mobile

## HTTP GET

Endpoint: `https://api.topup.monster/check/genshinimpact`

- os_usa = America
- os_euro = Europe
- os_asia = Asia
- os_cht = TW, HK, MO

```php
<?php

$curl = curl_init();

curl_setopt_array($curl, array(
  CURLOPT_URL => 'https://api.topup.monster/check/genshinimpact?user_id=xxx&zone_id=xxx&api_key=xxx',
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
