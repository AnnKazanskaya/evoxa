# EVOXA — Official Website

Профессиональная косметология. Производство в Барселоне.

## Стек

Чистый HTML / CSS / vanilla JS. Без сборщиков, без зависимостей, без бэкенда.
Один файл `index.html` + папка `images/`.

## Структура

```
.
├── index.html        # Весь сайт: HTML, CSS, JS в одном файле
├── images/           # Фото для всех разделов (25 файлов, ~2.5 МБ)
└── README.md
```

## Локальный запуск

Открыть `index.html` в браузере двойным кликом. Без сервера.

Или поднять локальный сервер для нормальной работы относительных путей:

```bash
cd evoxa-site
python3 -m http.server 8000
```

Открыть http://localhost:8000

## Что есть

- Главная с видео-фоном, манифестом, каталогом продуктов и редакционным разделом
- 4 продукта (PEEL 1, PEEL 2, PEEL 3, TONIC) — каждый с отдельной страницей
- Раздел «Где сделать» — поиск клиник по городам РФ и Испании
- Обучение — 8 онлайн-курсов с видео RuTube + 5 городов оффлайн-обучения
- Журнал
- Форма заявки для инфлюенсеров
- 3 языка: русский, английский, испанский
- Адаптив для мобильных
- Анимации: scroll-reveal, параллакс, кастомный курсор, count-up счётчики

## Деплой

### GitHub Pages

1. Repository → Settings → Pages
2. Source: Deploy from a branch → `main` → `/ (root)` → Save
3. Через 1-2 минуты сайт доступен по адресу `https://USERNAME.github.io/REPO_NAME/`

### Netlify (если нужен свой домен)

1. [app.netlify.com/drop](https://app.netlify.com/drop) — drag&drop папку с `index.html`
2. Готовый URL за 30 секунд
3. Свой домен — Settings → Domain Management

## Замена видео в курсах

Видео встроены через iframe RuTube. Чтобы заменить — открой `index.html`, найди константу `TRAINING` (поиск `const TRAINING = [`). У каждого курса есть поле `rutube` с URL embed-плеера. Замени URL — готово.

## Контакты

Evoxa Studio S.L.
Calle Bailen 62, 08009 Barcelona, España
info@evoxa.com
