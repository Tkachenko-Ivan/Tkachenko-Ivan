### Рад приветствовать всех на странице моего профиля 👋

Меня зовут Иван, и я погромист, на всяких языках программирования: 

![](https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Tkachenko-Ivan&theme=github)

Похвастаться тем, что я очень активный пользователь GitHub, не могу:

![](http://github-profile-summary-cards.vercel.app/api/cards/stats?username=Tkachenko-Ivan&theme=github)

Но профиль существует уже давно, и здесь всё же скопилось несколько публичных репозиторев, вот, статистика не даст соврать:

![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Tkachenko-Ivan&theme=github)

Поэтому опишу что есть в моих репозиториях на GitHub, может они будут чем-то полезны.

# Репозитории

## newsseacher

Пример CRUD контроллера, взаимодействующего с поисковиковым движком Manticore Search.

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=newsseacher)](https://github.com/Tkachenko-Ivan/newsseacher)

Подрбнее о работе с поисковиком можно посмотреть на wiki-странице проекта: 📘 [Хватит ждать индексации: делаем данные доступными для поиска мгновенно на Manticore Search](https://github.com/Tkachenko-Ivan/newsseacher/wiki/Хватит-ждать-индексации:-делаем-данные-доступными-для-поиска-мгновенно-на-Manticore-Search).

Для удобства тестирования проекта, на GitHub Gist выложил файлы для развётрывания Docker контейнеров, и конфигурирования Manticore Search:
* [file-docker-compose-yaml](https://gist.github.com/Tkachenko-Ivan/9c8f8b5f98c80f902905b618878486ad#file-docker-compose-yaml) - создание контейнеров с БД и поисковым движком, необходимых для тестирвоания работы сервиса
* [manticore-simple.conf](https://gist.github.com/Tkachenko-Ivan/9c8f8b5f98c80f902905b618878486ad#file-manticore-simple-conf) - конфигурация поисковика для поиска по заранее созданному индексу
* [file-manticore-realtime-conf](https://gist.github.com/Tkachenko-Ivan/9c8f8b5f98c80f902905b618878486ad#file-manticore-realtime-conf) - конфигурация Manticore Search для обновления индекса в реальном времени

[![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=9c8f8b5f98c80f902905b618878486ad)](https://gist.github.com/Tkachenko-Ivan/9c8f8b5f98c80f902905b618878486ad)

## graphhopper-reader-postgis

![Static Badge](https://img.shields.io/badge/GIS-yellowgreen)

Пример переопределения источника данных в GraphHopper. 

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=graphhopper-reader-postgis&show_owner=true)](https://github.com/Tkachenko-Ivan/graphhopper-reader-postgis)

Это клон репозитория:

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=mbasa&repo=graphhopper-reader-postgis&show_owner=true)](https://github.com/mbasa/graphhopper-reader-postgis)

В своём клоне я много всего переделал "под себя", но это частности, поэтому Pull Request делать не стал, для Pull Request, я сделал отдельный Fork:

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=graphhopper-reader-postgis-fork&show_owner=true)](https://github.com/Tkachenko-Ivan/graphhopper-reader-postgis-fork)

Fork сделал, а Pull Request - нет, но ничего, может ещё доберусь... 

Об этом репозитории написал публикацию 📙 [Как хранить сеть дорог в БД для построения маршрута?](https://habr.com/ru/articles/688556/), программа умеет считывать данные из некоторого источника и строить по ним граф дорог, для маршрутизации. Однако, помимо чтения эти данные необходимо как-то записывать, вторая часть моей публикации о том, как это сделать.

Для того, чтобы можно было повторить, то, что написано в публикации подготовил:

* Docker образ  с предзаполненной Базой Данных дорог, для тестирования маршрутизации и загрузки новых данных, Docker Hub: [road-data](https://hub.docker.com/r/tkachenkoivan/road-data)
![Docker Image Size](https://img.shields.io/docker/image-size/tkachenkoivan/road-data) ![Docker Pulls](https://img.shields.io/docker/pulls/tkachenkoivan/road-data) ![Docker Stars](https://img.shields.io/docker/stars/tkachenkoivan/road-data)




* Алгоритм обработки появления новой дороги в Базе Данных:

[![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=c2418a09c887e0baa0a823944d76e343)](https://gist.github.com/Tkachenko-Ivan/c2418a09c887e0baa0a823944d76e343)
  
* Репозиторий с примерами данных для загрузки и обработки, моделирует различные ситуации, описанные в публикации

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=shape-example-graphhopper)](https://github.com/Tkachenko-Ivan/shape-example-graphhopper)


## searchfonetic

Репозиторий по созданию Docker контейнера для тестирования фонетических алгоритмов.

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=searchfonetic)](https://github.com/Tkachenko-Ivan/searchfonetic)

Индексацию и поиск по адресам описал в двух публикациях: 
* 📙 [Интернационализация поиска по городским адресам. Реализуем русскоязычный Soundex на Sphinx Search](https://habr.com/ru/post/547652/)
* 📙 [Продолжаем интернационализацию поиска по адресам с помощью Sphinx или Manticore. Теперь Metaphone](https://habr.com/ru/post/550690/).

Помимо самого репозитория выложил:
  * Конфигурационный файл поисковой платформы

[![Gist Card](https://github-readme-stats.vercel.app/api/gist?id=354db31938f7ed4218ac5d20c7f9502b)](https://gist.github.com/Tkachenko-Ivan/354db31938f7ed4218ac5d20c7f9502b)

  * Образ с индексами в Docker Hub: [tkachenkoivan/searchfonetic](https://hub.docker.com/r/tkachenkoivan/searchfonetic)
![Docker Image Size](https://img.shields.io/docker/image-size/tkachenkoivan/searchfonetic) ![Docker Pulls](https://img.shields.io/docker/pulls/tkachenkoivan/searchfonetic) ![Docker Stars](https://img.shields.io/docker/stars/tkachenkoivan/searchfonetic)




## hopper-illustration

![Static Badge](https://img.shields.io/badge/GIS-yellowgreen)

Проект который я выложил в качестве иллюстрации к публикации 📙 [Как использовать GraphHopper для построения пешеходных маршрутов по собственным правилам](https://habr.com/ru/articles/545782/), именно поэтому он `illustration`, не более.

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=hopper-illustration)](https://github.com/Tkachenko-Ivan/hopper-illustration)

В проекте и публикации показано, как в GraphHopper создать собсвенные правила, по которым будет строиться граф, используемый для поиска маршрутов.

## Geodesic

![Static Badge](https://img.shields.io/badge/GIS-yellowgreen)

Решает прямую и обратную геодезические задачи, на сфере и на эллипсоиде вращения.

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=Geodesic)](https://github.com/Tkachenko-Ivan/Geodesic) 

Для решения задач на эллипсоиде использует [формулы Винсенти](https://en.wikipedia.org/wiki/Vincenty's_formulae). Но библиотеку я создавал не совсем для этого, а для того, чтобы находить точку пересечения двух [ортодромий](https://ru.wikipedia.org/wiki/Ортодромия) (ограниченных концами отрезка). Публикация об этом: 📙 [Изобретаю свой сложный способ поиска координат точки пересечения двух линий](https://habr.com/ru/articles/825066/)

## Polylines

![Static Badge](https://img.shields.io/badge/GIS-yellowgreen)

Строит пространсвенный индекс для полилиний заданных координатами.

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=Polylines)](https://github.com/Tkachenko-Ivan/Polylines)

## Tetris

Самый древний из всех моих проектов, его я написал ещё в университете, на втором курсе, в качестве курсовой работы по предмету "Объектно Ориентированное и Визуальное Программирование". 

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Tkachenko-Ivan&repo=Tetris)](https://github.com/Tkachenko-Ivan/Tetris)

Понятное дело что это не просто учебный проект, в типичном учебном проекте предполагается наличие определённой темы и соответсвующего этой теме задания, в курсовом проекте всё иначе: только общие требования, а задумка и реализация - авторские, именно поэтому я его и выделяю на фоне прочих учебных задач.

Собирал я его в Borland Delphi 7 - всё ещё работает. 

Кстати, в [релизах](https://github.com/Tkachenko-Ivan/Tetris/releases) есть скомпилированные файлы, - можно скачать и запустить .exe чтобы поиграться, а ещё есть вики проекта с описанием как это всё устроено: 📘 [Описание работы программы](https://github.com/Tkachenko-Ivan/Tetris/wiki/Описание-работы-программы).

# Посты

Иногда я пишу на Хабр, обо всяком, в тексте выше попадаются некоторые ссылки на публикации посвящённые проектам, но не все публикации про код, многие не выражаются в виде какой-то программы, или нет смысла создавать под них репозиторий или даже Gist, поэтому веделил отдельный блок на этой странице, в котором показаны 5 последних публикаций:

<!-- BLOG-POST-LIST:START -->
- [Изобретаю свой сложный способ поиска координат точки пересечения двух линий](https://habr.com/ru/articles/825066/?utm_campaign=825066&utm_source=habrahabr&utm_medium=rss)
- [Геоданные без регистрации и СМС](https://habr.com/ru/articles/785254/?utm_campaign=785254&utm_source=habrahabr&utm_medium=rss)
- [Признаюсь: я писал поддельный экран загрузки](https://habr.com/ru/articles/747224/?utm_campaign=747224&utm_source=habrahabr&utm_medium=rss)
- [Бэкенд разработка и БДСМ. Страсти по именованию, или Как назвать отдел?](https://habr.com/ru/articles/700222/?utm_campaign=700222&utm_source=habrahabr&utm_medium=rss)
- [Как хранить сеть дорог в БД для построения маршрута?](https://habr.com/ru/articles/688556/?utm_campaign=688556&utm_source=habrahabr&utm_medium=rss)
<!-- BLOG-POST-LIST:END -->

# LeetCode

[![LeetCode stats](https://leetcode-stats-six.vercel.app/api?username=tkachenko-ivan)](https://github.com/KnlnKS/leetcode-stats)

# Примечание

Свой профиль, т.е. этот файл, я оформил исключительно благодаря публикации: [Оформляем README-файл профиля на GitHub](https://habr.com/ru/articles/649363/), всем рекомендую.

<!--
**Tkachenko-Ivan/Tkachenko-Ivan** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
