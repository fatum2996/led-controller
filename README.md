# Плата для управления светодиодными лентами используя прошивку Rainbow

![board picture](board.PNG)
## Функционал платы
Плата позволяет управлять лентами с адресными светодиодами. Контроллером служит пульт LED2017-21key или внешние тактовые
## Монтаж платы
Допускается использовать 1 из 3-х ИВЭП на выбор
## Прошивка платы
1. Запрограммировать Arduino Nano с помощью ПО [rainbow-radio](https://not-there-yet)
2. Запрограммировать Arduino Mega 2560 Pro Mini с помощью ПО [rainbow](https://github.com/fatum2996/rainbow), задав правильные значения в конфигурационных файлах. Использовать ветку main
## Подключение платы
### Кнопки
1. Подсоединить тактовую кнопку управления режимами между контактами BTN\_MODE и GND 
2. Подсоединить тактовую кнопку управления мерцанием между контактами BTN\_SIN и GND
### Ленты
1. Подключить адресную ленту «звездное небо» к контактам 5V\_LED, GND и DATA\_STAR 
2. Подключить адресную ленту «кометы» к контактам 5V\_LED, GND и DATA\_CMT
### Питание
1. Подключить 12В на разъем X2

Выводы для дополнительных лент доступны на контактах A0-A4<br />
При использовании мощных лент желательно пропаять проводом 1 мм<sup>2</sup> контакты XS1-XS4
