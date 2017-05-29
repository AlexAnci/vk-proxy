# vk-proxy
Прокси-сервер для приложения ВКонтакте на Android

## Настройка приложения
1. Открываем приложение ВК, заходим в Настройки
2. В конце списка настроек нажимаем О программе
3. Тыкаем на собаку раз 20
4. Открываем стандартный номеронабиратель и пишем следующий код: `*#*#856682583#*#*`
5. Изменяем Домен API и Домен OAuth на свои
6. Пользуемся приложением без проблем

## Запуск прокси
- Скопировать файл `config.example.js` в `config.js` и изменить нужные данные
- Выполнить `npm install`
- Выполнить `npm start`
- Настроить nginx по примеру в `conf/nginx.conf`
- Настроить HTTPS, так как приложение без него работать не будет. Можно либо подключить [Cloudflare](https://www.cloudflare.com), либо сгенерировать сертификат через [Let's Encrypt](https://certbot.eff.org) и добавить его в nginx.