# NuxtTemplate

[Документация по проекту](documentation/readme.md)

[Чеклист](documentation/checklist.md)

Документация по nuxt доступна здесь: [Nuxt 3 documentation](https://nuxt.com/docs/getting-started/introduction)

Примеры элементов дизайна и реализованных компонентов доступны по адресу http://localhost:3000/styleguide

В исходном коде страница расположена здесь: pages/Styleguide.vue. На этой странице подключаются компоненты с примерами различных блоков. Открыв нужный блок можно посмотреть примеры.

## Используемые библиотеки

В проекте используются готовые библиотеки для реализации различного функционала.
Документацию по ним можно посмотреть по ссылкам.

- [Bootstrap 5](https://getbootstrap.com/) - сетка, инпуты и прочие элементы. JS часть используется довольно редко из-за недостаточного удобства, гибкости и недостаточного функционала.
- [floating-vue](https://github.com/Akryum/floating-vue) - используется для реализации выпадающих меню (при клике и наведении).
- [Swiper](https://swiperjs.com) - используется для реализации слайдеров. Готовые vue компоненты не используются из-за недостаточной гибкости. В проекте реализованы собственные компоненты в которых используется swiper в чистом виде.

## Наборы иконок:

- [heroicons](https://heroicons.com/)
- [Feather](https://feathericons.com/)
- [svgrepo](https://www.svgrepo.com/)

Для удобства исходный код иконок копируется и создается vue компонент в который размещается код иконки.

Иконки расположены здесь: `components/Icons`

Названия компонентов необходимо указывать с префиксом Icon для удобства работы с автокомплитом в IDE



## Установка

Открываем консоль и клонируем проект себе:

```bash
git clone git@github.com:enterprise-it-ru/nuxt-template.git nuxt-template
```

Переходим в папку в которую склонировался проект (в команде выше это greenspark-frontend)

```bash
cd nuxt-template
```

Устанавливаем зависимости:

```bash
npm install
```

Теперь нужно создать файл с переменными окружения. Для этого копируем файл .env.example и сохраняем его просто с именем .env

Скопировать можно с помощью команды:

```bash
cp .env.example .env
```

В этом файле при необходимости изменяем домен проекта и прочие настройки если они есть.

## Разработка

Запускаем сервер разработки. Он будет доступен по адресу `http://localhost:3000`

```bash
npm run dev
```

## Production

Для сборки проекта в боевом режиме используется команда:

```bash
npm run build
```

Локально можно запустить сервер и посмотреть как отрабатывает SSR и прочие возможности следующей командой:

```bash
npm run preview
```
