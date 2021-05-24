# SysOps
## Владислав Тетюшкин

22 года. 4,5 года работаю в IT.


-----

## Релевантные навыки
-   Большой опыт администрирования Linux (Debian-based и RedHat-based) и сервисов;
-   Опыт работы с облаками и оркестрация развертывания виртуальных машин в GCP, AWS, Azure (без использования Terraform);
-   Опыт развертывания Managed Kubernetes кластера в GCP (GKE) и AWS (ECS Fargate), контейнеризации приложений и их деплоя в облачный кластер (или локально с помощью Docker-compose, так же большой опыт пользования Docker Swarm);
-   Знаю что такое Git и IaaC;
-   Опыт развертывания и настройки Zabbix для сбора метрик, Grafana для рисования графиков, GrayLog для сбора логов и построения дашбордов;
-   Большой опыт работы с системой виртуализации VMware, могу с закрытыми глазами:
    -    подготовить хосты, 
    -    установить гипервизоры, 
    -    развернуть VMware vCenter,
    -    настроить DRS/HA кластер, 
    -    написать скрипты для автоматизации развертывания ВМ;
-   Большой опыт администрирования и проектирования сетей. Есть сертификат CCNA и прослушанные авторизованные курсы CCNP;
-   Опыт автоматизации сетевых задач на Cisco с помощью Python и Ansible;
-   Люблю рисовать схемы в Visio. Умею составлять документацию;
-   Опыт общения с англоязычной поддержкой, выжил один в Великобритании общаясь с шотландцами.

> CCNA: [Ссылка для проверки](https://www.certmetrics.com/cisco/public/verification.aspx?code=1FPR3M6FKDQ4173L)

-----

## Хочу
-   Быть на острие технической сингулярности;
-   Научится пользоваться инструментами крутых DevOps инженеров;
-   Поднять свой скилл программирования до приемлемого, выучить Python и Go;
-   Видеть зеленые индикаторы в системе мониторинга.

-----

<div style="page-break-after: always; visibility: hidden"> 
\pagebreak 
</div>

## Мои интересные проекты
Два моих проекта, о которых хочется рассказать:

**Автоматизация развертывания стендов** для проведения чемпионатов по сетям Cisco в Azure (примерно 40 рабочих стендов за полчаса) и их автоматическая проверка после завершения работы участников. 

Краткое описание работы:

1) Запуск скрипта, создающего нужное количество Resource Group для каждого участника. В скрипте указан Cloud-init, который скачивает bash скрипт для развертывания EVE-NG (платформа для виртуализации сетевого оборудования);
2) Скрипт разворачивает EVE-NG, скачивает образы виртуальных машин, саму лабораторную работу, настраивает права для учетных записей участников и запускает ВМ, параллельно логгируя действия в Telegram;

        Wed Sep 16 09:07:28 UTC 2020 👨🏻‍🦽 EVE-1257727496 - Deploy started
        Wed Sep 16 09:07:30 UTC 2020 🏓 EVE-1257727496 - Installing eve-ng...
        Wed Sep 16 09:13:20 UTC 2020 💾 EVE-1257727496 - Copying images...
        Wed Sep 16 09:13:34 UTC 2020 📦 EVE-1257727496 - Installing Docker...
        Wed Sep 16 09:14:50 UTC 2020 🏆 EVE-1257727496 - Deploy completed. Rebooting...
        Wed Sep 16 09:14:51 UTC 2020 🌎 EVE-1257727496 - My IP is 40.112.49.80

3) После выполнения работы участником, я запускаю автоматическую проверку задания, которая спрятана в Docker контейнере (Python скрипт), который предварительно собран с помощью GitHub Actions и залит в Registry.

> К сожалению этот репозиторий приватный и я не могу его показать...

Следующий проект - **автоматизация настройки VPN** по сертификатам на Cisco в сети крупной организации (~120 филиалов). Вся работа была поделена на четыре этапа:

1)  Подготовка данных о маршрутизаторах из неудобных экселек и сбор прочей информации;
2)  Выписывание сертификатов с Active Directory Certificate Authority на каждый маршрутизатор;
3)  Настройка первой и второй фазы IPSec на каждом маршрутизаторе и сохранение предыдущей конфигурации для отката;
4)  Тестирование соединений и проверка работоспособности туннелей.

Первые два этапа выполнены в виде Playbook'ов для Ansible, третий этап выполнен с помощью библиотеки pyATS для Python (в парсерах которой я нашел ошибки и создал issue).

>GitHub Repo этого [проекта](https://github.com/Lawliet2012/dmvpn-move-to-rsa "dmvpn-move-to-rsa")

-----

<div style="page-break-after: always; visibility: hidden"> 
\pagebreak 
</div>

## Немного о себе

Очень интересна работа с облаками, в особенности AWS и GCP. Также горизонтальное масштабирование, репликации и кластеры баз данных, в общем всё, что связано с Highload и современными сервисами.

Могу похвастаться, что являюсь призером международных чемпионатов по "Сетевому и системному администрированию":

- EuroSkills 2018 г. Будапешт - золото;
- Global Skills Challenge 2019 г. Мельбурн - золото;
- WorldSkills International 2019 г. Казань - медальон за профессионализм;
- И еще куча других тренировочных чемпионатов в разных странах (Япония волшебна, а в Великобритании подают странный [соус](https://en.wikipedia.org/wiki/HP_Sauce)).

Имею Почетную грамоту президента РФ.

Контакты:
-   Tg: @Lawliet1
-   Tel: +79995597590
-   Mail: lawliet2012sven@gmail.com

-----