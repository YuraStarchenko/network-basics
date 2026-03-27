# Day 2 — DNS + HTTP + Wireshark

## Что я понял

DNS переводит имя сайта в IP-адрес.  
HTTP используется для общения браузера с сервером.

## DNS

- google.com → (твой IP)
- youtube.com → (твой IP)

![DNS nslookup](screenshots/dns_nslookup.png)

## HTTP

- Ответ сервера: 200 OK

![HTTP curl](screenshots/http_curl.png)

## Wireshark

### DNS

Я увидел, как компьютер отправляет запрос к DNS серверу и получает IP.

![Wireshark DNS](screenshots/wireshark_dns.png)

### HTTP

Я увидел GET-запрос и ответ сервера.

![Wireshark HTTP](screenshots/wireshark_http.png)

## Вывод

(напиши своими словами)
