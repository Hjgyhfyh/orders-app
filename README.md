# orders-app — витрина заказов (Telegram Mini App)

Одностраничная витрина услуг для приёма заявок на разработку. Чистый HTML/CSS/JS, без сборщиков.

## Что это
Telegram Mini App «витрина заказов»: услуги с ценами, «как это работает», честный блок про Roblox и форма заявки. Строго чёрно-белый студийный дизайн (Unbounded + Inter, grain, стеклянные карточки, плавные появления).

## Услуги
- Roblox-скрипт — от 300₽
- Telegram-бот — от 500₽
- Сайт / лендинг — от 800₽
- Парсер — от 500₽
- Презентация — от 800₽
- Приложение — от 1000₽

## Как открыть
- **В Telegram:** привязать URL этой страницы к боту `@teststsbbot` (menu button или web_app-кнопка).
- **В браузере:** просто открыть https://hjgyhfyh.github.io/orders-app/ — работает и без Telegram API.

## Отправка заявки
Собирается JSON `{service, game, brief, budget}`:
- если Mini App запущен с reply-кнопки — `tg.sendData(...)` + `tg.close()`;
- иначе (menu button / браузер) — открывается чат бота `https://t.me/teststsbbot?start=app_<service>` с подсказкой отправить описание.

Дизайн: фон всегда `#000`, тема Telegram игнорируется (`setBackgroundColor`/`setHeaderColor`). MainButton — белая на чёрном.

## Связь
[@sigmatik323](https://t.me/sigmatik323)
