## Мои шаблоны Gulp в динамике развития

## Проект <Имя проекта>

### Для создания нового проекта по этому шаблону введите **_npm i_**

### В файлах \*.scss не используйте однострочные комментарии

Вместо " // " следует использовать " /\* \*/ ", иначе получим ошибку !

### Корень проекта для указания путей в html, css, js файлов - это src. При указании абсолютного пути src не указывается, а применяется следующий синтаксис: "/css/style.min.css" или "/js/main.min.js"

Это особенно важно при сборке html-файлов из отдельных частей. Данный синтаксис позволяет адресоваться к нужному файлу вне зависимости от того, в какой папке мы находимся - это УНИВЕРСАЛЬНЫЙ СИНТАКСИС для указания одних и тех же частей html-файлов для сборки html-файлов, находящихся в различных подпапках.

### Напротив, для указания путей в файле gulpfile.js, корневым является имя проекта и применяется следующий синтаксис: 'src/css/\*.css'

### Со стилями работаем в папке SCSS (папку CSS не трогаем!).

### С html-файлами работаем в папке HTML_PAGES (не трогаем папку HTML_RESULT, а, тем более, файл index.html в корне папки SRC - они генерируются автоматически).

### Проект для передачи в production находится в папке DIST в корне проекта. Его обновление не автоматизировано и выполняется командой "GULP BUILD".

### В блоках head.html и foot.html осуществлены подключения

1. Файла стилей style.css
2. Файла нормализация стилей normalize.css
3. Файла main.js
4. Библиотеки Swiper
5. Библиотеки Fancybox
