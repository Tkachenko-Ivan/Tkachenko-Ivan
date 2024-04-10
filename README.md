### Всем привет 👋

# Проекты

Опишу что есть в моём профиле на GitHub, может он будет чем-то полезен.

* [newsseacher](https://github.com/Tkachenko-Ivan/newsseacher) - пример создания CRUD-контроллера для взаимодействия с поисковым движком. Подрбнее о работе с поисковиком можно посмотреть на wiki-странице проекта: [Хватит ждать индексации: делаем данные доступными для поиска мгновенно на Manticore Search](https://github.com/Tkachenko-Ivan/newsseacher/wiki/Хватит-ждать-индексации:-делаем-данные-доступными-для-поиска-мгновенно-на-Manticore-Search)

* [graphhopper-reader-postgis](https://github.com/Tkachenko-Ivan/graphhopper-reader-postgis) - это клон репозитория [mbasa/graphhopper-reader-postgis](https://github.com/mbasa/graphhopper-reader-postgis), в котором я много всего переделал "под себя", но это частности, поэтому Pull Request делать не стал, для Pull Request, я сделал отдельный Fork [graphhopper-reader-postgis-fork](https://github.com/Tkachenko-Ivan/graphhopper-reader-postgis-fork). Fork сделал, а Pull Request - нет, но ничего, может ещё доберусь... Об этом репозитории написал публикацию [Как хранить сеть дорог в БД для построения маршрута?](https://habr.com/ru/articles/688556/). программа умеет считывать данные из некоторого источника и строить по ним граф дорог, для маршрутизации. Однако, помимо чтения эти данные необходимо как-то записывать, вторая часть моей публикации о том, как это сделать, а так же:
  * в Docker Hub: [road-data](https://hub.docker.com/r/tkachenkoivan/road-data) - образ с предзаполненной Базой Данных дорог, для тестирования маршрутизации и загрузки новых данных 
  * в GitHub Gist: [Сервис обработки новых данных](https://gist.github.com/Tkachenko-Ivan/c2418a09c887e0baa0a823944d76e343) - показан алгоритм обработки новой дороги в Базе Данных
  * в GitHub: репозиторий [shape-example-graphhopper](https://github.com/Tkachenko-Ivan/shape-example-graphhopper) - с примерами данных для загрузки и обработки, моделирует различные ситуации, описанные в публикации

* [searchfonetic](https://github.com/Tkachenko-Ivan/searchfonetic) - этот проект - пример кофигурации поисковика для работы с адресами. Индексация и поиск по адресам описаны в двух публикациях: [Интернационализация поиска по городским адресам. Реализуем русскоязычный Soundex на Sphinx Search](https://habr.com/ru/post/547652/) и [Продолжаем интернационализацию поиска по адресам с помощью Sphinx или Manticore. Теперь Metaphone](https://habr.com/ru/post/550690/). Помимо самого репозитория выложил:
  * в GitHub Gist: [Конфигурационный файл поисковой платформы](https://gist.github.com/Tkachenko-Ivan/354db31938f7ed4218ac5d20c7f9502b)
  * в Docker Hub: [Образ с индексами](https://hub.docker.com/r/tkachenkoivan/searchfonetic)

* [hopper-illustration](https://github.com/Tkachenko-Ivan/hopper-illustration) - проект который я выложил в качестве иллюстрации к публикации [Как использовать GraphHopper для построения пешеходных маршрутов по собственным правилам
](https://habr.com/ru/articles/545782/), менно поэтому он `illustration`, не более. В проекте и публикации показано, как в [GraphHopper](https://github.com/graphhopper/graphhopper/tree/0.10) создать собсвенные правила, по которым будет строиться граф, используемый для поиска маршрутов.

* [Geodesic](https://github.com/Tkachenko-Ivan/Geodesic) - решает прямую и обратную геодезические задачи, на сфере и на эллипсоиде вращения. Для решения задач на эллипсоиде использует [формулы Винсенти](https://en.wikipedia.org/wiki/Vincenty's_formulae). Но библиотеку я создавал не совсем для этого, а для того, чтобы находить точку пересечения двух [ортодромий](https://ru.wikipedia.org/wiki/Ортодромия) (ограниченных концами отрезка).

* [Polylines](https://github.com/Tkachenko-Ivan/Polylines) - строит пространсвенный индекс для полилиний заданных координатами.

# Статистика по проектам

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Tkachenko-Ivan)](https://github.com/anuraghazra/github-readme-stats)

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
