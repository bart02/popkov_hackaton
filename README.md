# Система навигации беспилотного автомобиля по карте
## Команда
![Providence](https://user-images.githubusercontent.com/19249148/83388209-40b51100-a418-11ea-9172-59449ab0a016.png)
- Артём Баталов ([batalov.me](http://batalov.me/))
- Карина Янышевская (Telegram: [@Fanot1](http://t.me/Fanot1))
- Игорь Сидорин (Telegram: [@maerans](http://t.me/maerans))
- Тимофей Валов (Telegram: [@timofius3](http://t.me/timofius3))

## Суть проекта
На этом хакатоне мы решили разработать удобную масштабируемую систему для навигации робоавтомобиля.

Пользователь отмечает любую точку на редактируемой карте, после чего робоавтомобиль сам прокладывает до нее оптимальный маршрут, учитывая плотность траффика. Однако, наша система не идеальна, и как и в любой неидеальной системе - присутствуют неавтономные элементы. Так для проезда пилотируемого автомобиля присутствует шлагбаум, который может быть открыт человеком.

## Применение
Самый очевидный пример применения такой технологии - грузовой склад. Целый штат водителей погрузчиков может быть заменен одним оператором за пультом, при этом минимизируется риск ошибки за счет присутствия человека вместо искусственного интелекта. Полезно там, где по причинам высокой ценности груза процесс не может регулироваться автоматически.

Еще, эта технология имеет потенциал в сфере развлечений, прежде всего для детей. Это может быть реализовано, например, в виде специальной стилизованной тележки, в кабине которой ребенок не скучает в магазине или аэропорту, при этом у родителей нет причин для беспокойства: весь маршрут ребенка известен, риск потери минимизирован. Точно таким же образом могут быть организованы детские аттракционы

Еще одним кейсом применения нашей разработки будут системы умного дома. При покупке робота-помошника в систему умного дома пользователь строит граф - карту помещения, и используя нашу технологию, размечает маршруты, по которым робот в дальнейшем совершает рутинные действия, например приносит воду или открывает окна.

## Перспективы развития
Во-первых, необходимо реализовать более точное отслеживание пробок. На данный момент в система используется принцип “занятость точек”, который не является эффективным при использовании наземного пространства. Из этого следует необходимость использования системы навигации (indoor- или outdoor-) в зависимости от кейса использования устройства.

Во-вторых, расширить использование специальных систем (по типу реализованного шлагбаума) для включения в систему неавтономных элементов.

И конечно, провести более подробное исследование рынка для выделения основных задач дальнейшей разработки системы.

## Видео защиты проекта
[![YouTube](https://user-images.githubusercontent.com/19249148/83399671-ca220e80-a42b-11ea-8371-e23431a3568d.png)](https://youtu.be/0_JZH24qXas)

## Источники кода
- Код стрима и просмотрщика - https://raspberrypi.stackexchange.com/a/87815
- Веб портирован с https://github.com/Tennessium/HUEX
- Движение робоавтомобиля по линии - https://github.com/bart02/NTIcar
