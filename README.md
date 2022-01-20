# **Geolocation by IP**

В нашем распоряжении CSV-таблица (**[link](https://www.dropbox.com/s/wo0dexr0p3q4fgb/IP2LOCATION-LITE-DB1.CSV?dl=0)**), в которой длинный перечень строк с диапазонами IP-адресов (от и до  — 1-й и 2-й столбец соответственно), а также страной, которой выданы эти IP.

Задача заключается  в том, чтобы написать веб-приложение на Express, выделив ендпоинт, по которому размещённый на сервере алгоритм сможет определять, откуда постучался пользователь и возвращать ему и значение IP-адреса, и страну, с которой был осуществлён запрос.

- **Приложение должно уметь:**
    - *определять IP-шник юзера по переходу*
    - *определять локацию юзера по IP-шнику, используя CSV-базу*
    - *возвращать юзеру диапазон адресов (в «человеческом» понятном виде) и страну по таблице*

### 👆 **Как себя проверить?**

Вот список IP-адресов, которые выделены на конкретные страны. Если всё сделано верно, то скрипт должен успешно возвращать response (или для старта выводить в консоль), указывая на правильную страну при отправке айпишника в Body запроса:

>
```
Armenia — 185.182.120.34
Mexico — 45.177.176.23
Turkey — 5.44.80.51
Norway — 91.149.48.22
Cyprus — 203.24.108.65
UK — 23.43.23.15
Ireland — 89.28.176.5
Romania — 77.83.248.211
```
> 

Для проверки также можно установить Ngrok и поиграться с Proxy, стучась на открытый нгроком адрес.
