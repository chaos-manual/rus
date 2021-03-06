# Уязвимости, атаки и патерны решений

В своей практике мы используем практически все известные на данный
момент атаки, которые существуют в методологии Chaos Engineering:
хостовые, ресурсные, Network, AZ-атаки, региональные атаки. 

Но когда мы работаем в компании до 10-15 команд и
общая численность команд составляет не более 200 человек, данные атаки
можно проводить практически без подготовки. И как только мы сталкиваемся
с ситуацией, что у нас в компании/команде больше 5000 узлов или нод на
приходится одну автоматизированных систем, а 5000 нод это всего лишь
один кластер для стресс-испытаний и с этим кластером работает 18 команд,
а в организации таких автоматизированных систем по размеру, более 100 и
300, то такие атаки проводить очень сложно.

Поэтому изначально требуется разбить атаки на несколько этапов. Каждые
атаки имеют свой вес. Этапы добавляют в нашу методику новую грань, на
примере системы координат к осям **X** и **Y** необходимую ось **Z** и
делают ее трёхмерной для таких сложных систем и команд.

В первый этап можно включить атаки ресурсные по CPU, RAM поскольку их
проводить легче, и они запускаются на кластерах просто и
массово.

Атаки, связанные с интеграцией, требуют больше подготовки, и мы их
должны проводить в определенной зрелости команды и системы. Этому будет
посвящена в нашем Manual отдельный раздел, в котором мы достаточно
глубоко рассмотрим типы атак и как их можно разбить на группы, к каким
приступать в первую очередь и каким приступать поэтапно, когда
развивается командам прошедшая определённый путь и культура Chaos
Engineering стала сильнее в команде.


После того как мы провели атаки, мы обычно получаем отчет с
результатами. На базе протоколов у нас есть точки отказов, где система
может сломаться. В данных точках отказа требуется провести большую
работу. Чаще всего нас спрашивают: каким образом можно работать с этой
точкой отказа? На самом деле тот результат, который мы получаем, это не
дефект с которым нужно бежать и сразу его править в конкретной понятной
точке. Чаще всего в этой точке нужно будет поработать команде, которая
проводит разработку, которая сопровождает систему возможно Solution
архитектору. В нашей методологии, в нашем Manual, есть отдельная глава,
которая описывает как раз такие процедуры детальные рассмотрение этих
точек отказа и потенциальных точек отказа.


Далее на базе этих точек мы должны научиться с ними работать и в итоге
мы можем как минимум развить какие-то параметры на мониторинге,
доработать fails-check, сделать редизайн какого-то сервиса. Чаще всего
требуется, в случае с конкретным приложением или сервисом, сделать его
не ре-дизайн, а именно доработать те инструменты, которые позволят
системе быть более надежной. На текущий момент к разработчикам
предъявляется требование не только по написанию бизнес-функций, а и
тому, как этот бизнес-сервис будет жить на какой-то конкретной
инфраструктуре, как он будет работать в высокие сезоны, либо при высоких
нагрузках, во время высоких нагрузок плюс каких-то дизастров на
инфраструктуре не только. Ну и конечно же возможно потребуется доработка
определённых балансировщиков. Все эти блоки мы будем рассматривать
подробно в соответствующих разделах Manual.

Блок "**Уязвимости, атаки, паттерны решений"** хочется закончить тем,
что существует огромное количество паттернов, которые применяются при
разработке софта. И Chaos Engineering способствует тому, чтобы
разработчики использовали более активно эти паттерны и писали более
оптимальные системы.

---

Learn about types of fault injections - the standard list of fault injections (also known as attacks) can be [found here](https://www.gremlin.com/docs/infrastructure-layer/attacks/). We follow a slightly different grouping that enables us to prioritize complexity and costs of staging the tests.

### Обсуждение

- уязвимости (свойства системы в конкретных условиях эксплуатации)
- аттаки - способы тестироваия  
- паттерны решений в привязке с атаками или уязвимостями
  (даем пример "Out of memory c Web-SPHERE")
- см.также glossary  

