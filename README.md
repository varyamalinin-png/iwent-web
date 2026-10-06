# ДЗ №1. HTML + CSS — вёрстка веб-приложения GreenNest

GreenNest — веб-приложение для садоводов: каталог семян, обмен семенами, подписка на сезонные наборы, запись на садовые услуги, трекер растений, программа эко-баллов, корзина, вход и регистрация.

**Исходные макеты:** [GreenNest — Figma Community](https://www.figma.com/community/file/1623942260962687765/greenest)

**Вёрстка (живые страницы):** https://varyamalinin-png.github.io/iwent-web/

**Исходники вёрстки:** [index.html](index.html) и остальные файлы в этой ветке

## Экраны

| Экран в макете | Страница |
|---|---|
| HOME PAGE | [index.html](index.html) |
| Seeds | [seeds.html](seeds.html) |
| Seed Exchange program | [seed-exchange.html](seed-exchange.html) |
| Subscription Box | [subscription.html](subscription.html) |
| Subscription payment | [subscription-payment.html](subscription-payment.html) |
| Gardening Services | [services.html](services.html) |
| Book Services | [book-service.html](book-service.html) |
| Plant tracker | [plant-tracker.html](plant-tracker.html) |
| Add new plant | [add-plant.html](add-plant.html) |
| Fertilizers | [fertilizers.html](fertilizers.html) |
| Eco Points | [eco-points.html](eco-points.html) |
| Cart | [cart.html](cart.html) |
| Sign in | [sign-in.html](sign-in.html) |
| Join GreenNest | [sign-up.html](sign-up.html) |

Страницы связаны между собой: меню, кнопки и ссылки ведут на соответствующие экраны.

## Структура проекта

```
index.html, *.html   — страницы приложения
css/styles.css       — общие стили
img/                 — изображения и иконки из макета
```

## Выполнение критериев

| Критерий | Реализация |
|---|---|
| Ссылка на вёрстку и исходные макеты | В начале этого файла |
| Семантические теги | `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`, `address`, `form`, `fieldset` / `legend`, `label`, `output`, `time`, `dl` / `dt` / `dd`, списки `ul` для карточек и меню |
| CSS-переменные | Блок `:root` в начале `css/styles.css`: палитра, градиенты, шрифт, шкала размеров текста, ширина контейнера, отступы, радиусы, тени. Ширина полосы прогресса задаётся переменной `--value`, число колонок формы — `--cols` |
| Стили задаются классами | Все компоненты стилизуются через классы (БЭМ). Селекторы по тегам используются только в базовом сбросе |
| Названия классов по бизнес-смыслу | `seed-card`, `catalog-filters`, `offer-card`, `plan-card`, `order-summary`, `payment-method`, `service-card`, `booking-card`, `plant-card`, `impact-card`, `reward-card`, `activity-list`, `milestone`, `fertilizer-card`, `assistant-chat`, `empty-state`, `cart-link` |
| Flex / Grid | Grid: сетки карточек (семена, услуги, растения, награды, предложения обмена, тарифы), каталог с фильтрами, раскладка страницы эко-баллов, строки форм, подвал. Flex: шапка и меню, кнопки, заголовки страниц, содержимое карточек |
| Соответствие макету | Структура экранов, тексты, изображения, цвета и пропорции перенесены из макета |
| Адаптивность | ≥ 1024 px — десктоп по макету; 768–1023 px — планшет: меню в бургере (чистый CSS), сетки в 2 колонки, фильтры каталога над карточками; < 768 px — мобильная версия в одну колонку |

## Запуск

Открыть `index.html` в браузере, сборка не требуется.
