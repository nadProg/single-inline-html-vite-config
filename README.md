1. Разворачиваем проект:
```
npm create vite@latest my-project -- --template vanilla-ts
```
   Для разработки на чистом javascript используем шаблон `vanilla`. Подробнее [тут](https://vitejs.dev/guide/#trying-vite-online).

2. Устанавливаем плагины `vite-plugin-html` и `vite-single-file` и добавляем их в конфигурацию `vite.config.js`.

3. Плагин `vite-single-file` вставляет инлайном все скрипты, подключенные к `index.html`, и все стили, которые туда импортируются. Все стили и код минифицируются этим же плагином.

4. Плагин `vite-plugin-html` минифицирует оставшийся `html`.

5. Для разработки запускаем проект `npm run dev`.

6. Для сборки запускаем `npm run build`. Проект собирается в папку `/dist`.

