---
title: Что я использую в работе
date: 2023-01-01 00:00:00
categories: node_modules
tags:
  - NodeJS
---

Однажды на собеседовании меня спросили какие модули я использую в работе. Вопрос был неожиданным и я что-то промлямлил. Тогда я и решил собрать список.

# NodeJS
## Модули

* [dotenv](https://www.npmjs.com/package/dotenv) - модуль для чтения конфигурации из .env файлов или переменных окружения. Будет полезен если вы будете оборачивать свою программу в Docker.
* [cheerio](https://www.npmjs.com/package/cheerio) - Обход html как в jQuery, только без браузера
* [alasql](https://www.npmjs.com/package/alasql) - обращение к csv/xls, массивам/объектам через SQL запросы
* [node-cron](https://www.npmjs.com/package/node-cron) - если нужно выполнять задачи по крону
* [rimraf](https://www.npmjs.com/package/rimraf) - кроссистемная очистка каталога dist.
* [ioredis](https://www.npmjs.com/package/ioredis) - более быстрая реализация клиента для Redis
* [Helmet](https://www.npmjs.com/package/helmet) - Защита REST API
* [fs-extra](https://www.npmjs.com/package/fs-extra) - Улучшенный модуль fs
* [NodeMailer](https://www.npmjs.com/package/nodemailer) - Отправка писем
* [winston](https://www.npmjs.com/package/winston) - логгер, который имеет возможность экспорта сообщений в разные места. Например, в Graylog, Telegram.
* [winston-error](https://www.npmjs.com/package/winston-error) - плагин для winstone, который позволяет проще сообщать ошибку
* [winston-transport-sequelize](https://www.npmjs.com/package/winston-transport-sequelize) - Отправка логов в БД через ORM Sequelize
* [bcrypt](https://www.npmjs.com/package/bcrypt) - Для хэширования паролей и прочего.

# Приложения:
## Для Redis
* [Redis Desktop Manager](https://github.com/uglide/RedisDesktopManager) - испольовал этот GUI Для Redis ранее;
* [resp.app](https://resp.app/) - GUI для Redis;
## Другое
* [dBeaver](https://dbeaver.io) - GUI для MysqlPostgres и др

# Плагины VSCode:
* ESLint - Линтер
* Peacock - используюего для раскраски различных проектов. Так проще их различать. Например работу и свой Пет проджект.
* Prettier - делает ваш код красивым и единообразным согласно правилам принятым в компании
* Tabnine - AI плагин, который анализирует текущий проект и подставляет вам код
* EJS Language Support - поддержка ejs в редакторе
* ejs Snippets -предлагает сниппеты, если вы пользуетесь ejs

