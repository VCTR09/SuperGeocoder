<a id="anchor"></a>
# Super Geocoder

### Geography Web App

[ссылка на сайт приложения: <img width="345" alt="link" src="https://user-images.githubusercontent.com/97599612/173211522-0ea8ed77-c1d2-4ae3-a4d0-071e2c4911bb.png">](http://geocoder123.pythonanywhere.com/)


_Библиотеки, использованные при создании приложения:_
```
from flask import Flask, render_template, request, send_file
from geopy.geocoders import ArcGIS
import pandas
import datetime
import folium
```


Загрузите _CSV_-файл в котором есть колонка _«Address/address»_ с адресами мест на сайт. Серверная часть приложения - _Python_ скрипт cчитывает файл и добавляет значения широты и долготы к каждому из мест.


Таблица результатов отображается на веб-странице, при нажатии пользователем кнопки _«Submit»_. После чего _CSV_-версия файла, содержащаю данные широты и долготы станет доступна для скачивания.


При нажатии на кнопку _«Map»_, которая отобразится под таблицей, будет показана интерактивная карта местности с адресами из таблицы показанными на карте в качестве меток. 

При загрузке неподходящего файла (например, без столбца _«Address»_), будет показано сообщение: _«Please make sure you have an address column in your CSV file!»_.
___


:earth_africa: *Главная страница приложения: После выбора файла, нажмите кнопку __"Submit"__.*
<img width="1440" alt="screen1" src="https://user-images.githubusercontent.com/97599612/173211317-1568a754-1b7b-4811-8438-35f14b22c80c.png">

:earth_americas: *На главной странице отобразится Ваша дополненная таблица со столбцами Широты и Долготы - __"Latitude"__ & __"Longitude"__. Данную таблицу можно скачать на свое устройство, нажав на кнопку __"Download"__. При нажатии на кнопку __"Map"__ все адреса из таблицы будут показаны на интерактивной карте.*
<img width="1440" alt="screen2" src="https://user-images.githubusercontent.com/97599612/173211322-3291772a-e432-4277-86b7-8978900890e3.png">

:globe_with_meridians: *Интерактивная карта с адресами из таблицы.*
<img width="1427" alt="screen3" src="https://user-images.githubusercontent.com/97599612/173184171-3e163fde-adc2-4599-b17b-514b52a66a87.png">

:balloon: *Всплывающее окно с указанием адреса.*
<img width="1423" alt="screen4" src="https://user-images.githubusercontent.com/97599612/173184175-03287e75-9c65-4e9b-b756-ed16f45c657e.png">

:file_folder: *Скачанный CSV файл (__yourfile.csv__) доступен в папке Загрузок.*
<img width="752" alt="screen5" src="https://user-images.githubusercontent.com/97599612/173184803-d3760f87-0c88-42f6-a90a-f088a3501acb.png">


[Вверх](#anchor)
