# DataHeroes Desktop App

## 1. Desktop-Master

```
Задачи мастера: авторизация и конфигурация Desktop-App

Предполагается, что после установки на локальную машину: Windows, Linux, Mac
Desktop-App потребует ввода лицензионного ключа
По данному лицензионному ключу осуществляется авторизация и идентификация конкретного клиента, который использует Desktop-App.
После успешной авторизации Master передает на Desktop-App конфигурацию:
1. К какой БД и как подключиться на локальной машине
2. Имена таблиц и имена столбцов, с которых необходимо получать данные
3. Обратный адрес: вебхук

Стек:
Nestjs
Expressjs
Postgresql + Typeorm
```

## 2. Desktop-App

```
Задача Desktop-App - обеспечить получение основной системой данных из локальной базы данных
Desktop-App - unix daemon, windows - service, должен быть встроен в автозагрузку
GUI при запуске через файл - HTML + Vuejs

Cтек:
Nodejs + Inversify
Любая локальная БД, к которой коннектимся через конфиг
Важные библиотеки: 
nexe: https://www.npmjs.com/package/nexe
node-windows: https://www.npmjs.com/package/node-windows
node-mac: https://www.npmjs.com/package/node-mac
node-linux: https://www.npmjs.com/package/node-linux

```
