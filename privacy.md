---
title: Политика конфиденциальности «Смета» / Smeta Privacy Policy
permalink: /privacy/
---

# Политика конфиденциальности расширения «Смета»

_Последнее обновление: 20 ноября 2026 г._

«Смета» — расширение для Google Chrome для учёта подписок. У расширения нет собственного сервера: разработчик не получает, не хранит и не передаёт ваши данные.

## Какие данные обрабатываются

| Данные | Зачем | Где обрабатываются |
|---|---|---|
| Подписки, которые вы вводите (название, стоимость, срок, заметки), и настройки | Показать список, итоговую сумму, сроки и советы | Только в вашем браузере (`chrome.storage.local`) |
| История посещений за последние 90 дней | Найти знакомые подписочные сервисы и предложить их добавить | Только на устройстве. Сохраняется лишь подсказка: название сервиса и число визитов |
| Отправитель и тема писем в Gmail (без текста писем) | Найти письма о продлении и оплате подписок | Только на устройстве |
| Временный токен доступа Gmail (если вы сами подключили Gmail API) | Прочитать заголовки писем через Gmail API | В памяти сессии браузера (`chrome.storage.session`). Удаляется при закрытии браузера или по кнопке «Отключить» |

## Передача данных

- Расширение не отправляет данные разработчику или третьим лицам.
- Если вы подключаете Gmail API, запросы идут из вашего браузера напрямую в Google (`gmail.googleapis.com`) по вашему собственному OAuth Client ID. Используется область доступа `gmail.metadata`: только заголовки писем, без содержимого.
- В расширении нет рекламы, аналитики и трекеров. Данные не продаются и не используются для оценки кредитоспособности.

Использование и передача информации, полученной из API Google, соответствует [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), включая требования Limited Use.

## Хранение и удаление

Данные хранятся, пока установлено расширение. Удалить их можно в любой момент: «Настройки → Очистить всё» или удаление расширения. Перед удалением можно сохранить копию кнопкой «Скачать копию».

## Контакты

Вопросы о конфиденциальности: [github.com/dima1380/smeta/issues](https://github.com/dima1380/smeta/issues)

---

# Smeta Privacy Policy

_Last updated: November 20, 2026_

Smeta is a Chrome extension for tracking subscriptions. It has no server: the developer does not receive, store or share any of your data.

**Data handled, all locally in your browser:**
- **Subscriptions and settings you enter:** stored in `chrome.storage.local`.
- **Browsing history (last 90 days):** matched on-device against a built-in list of subscription services. Only the resulting suggestion (service name and visit count) is stored.
- **Gmail sender and subject lines (never message bodies):** used to suggest subscriptions and processed on-device.
- **Gmail access token** (only if you connect the Gmail API yourself): kept in `chrome.storage.session` and cleared when the browser closes.

**Sharing:** none. Optional Gmail API requests go directly from your browser to Google using your own OAuth Client ID and the read-only `gmail.metadata` scope. No ads, analytics or trackers. Data is never sold or used for creditworthiness or lending.

Smeta's use and transfer of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements.

**Deletion:** Settings → "Очистить всё" (Clear all), or uninstall the extension.

**Contact:** [github.com/dima1380/smeta/issues](https://github.com/dima1380/smeta/issues)
