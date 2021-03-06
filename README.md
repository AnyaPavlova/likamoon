# startpack-less
Простой сборщик на less

**Version 1.0.5**

## Требования

Для работы необходимы

* [Node.js](http://nodejs.org) `последней версии LTS`
* [Gulp](http://gulpjs.com/): `[sudo] npm install -g gulp`

## Начало работы

**Форкнуть себе этот репозиторий и далее сколнировать свой форк!**

1 Клонируем с указанием названия папки проекта (название проекта в конце через пробел):
```
$ git clone git@github.com:your-login-on-github/student-startpack.git project-name
```

2 Избавляемся от привязки к удаленному репозиторию:
```
git remote rm origin
```

3 Создаем пустой репозиторий на github под проект

4 Привязываем наш проект к созданному удаленному репозиторию на github (пример команды):
```
git remote add origin git@github.com:your-login-on-github/name-repo.git
```

5 Пушим в удаленный репозиторий на github:
```
git push -u origin master
```
6 Ставим зависимости:
```
npm install
```

## Запуск

В консоли выполняем команду:
```
gulp serve
```
* Поднимается localhost
* В браузере автоматом открывается index.html
* Происходит отслеживание изменений в less файлах и их пересборка
* Происходит отслеживание изменений в html файлах
* При изменении происхожит перезагрузка страницы

## Структура папок и файлов
```
project
├───src
│   └───css
│       ├───blocks (стили блоков)
│       │   ├───_header.less
│       │   ├───_nav.less
│       │   └───etc.
│       │
│       ├───common (общие стили)
│       │   ├───_fonts.less
│       │   ├───_variables.less
│       │   └───etc.
│       │
│       └───style.less
│
└───www
    ├───fonts
    │   ├───font.woff2
    │   └───font.woff
    │
    ├───img
    │   ├───img.jpg
    │   └───etc.
    │
    ├───scripts
    │   ├───script.js
    │   └───etc.
    │
    ├───css
    │   ├───style.css (собранный из less файлов - его не трогаем)
    │   └───etc.
    │
    ├───index.html
    ├───page1.html
    └───etc.
```

## Версии
* 1.0.5 - расширенное описание как правильно стянуть в свой проект этот стартовый репозиторий
* 1.0.3 - добавлены читабельные сообщения об ошибках в консоли и окне уведомлений. Плагин - gulp-notify
* 1.0.0 - создание сборки
