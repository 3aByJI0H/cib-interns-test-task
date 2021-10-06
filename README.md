# Sock-Registration-Service

Реализовано приложение для автоматизации учёта носков на складе магазина. Кладовщик должен иметь возможность:

- учесть приход и отпуск носков;
- узнать общее количество носков определенного цвета и состава в данный момент времени.

Внешний интерфейс приложения представлен в виде HTTP API REST.
За более подробным описанием можно обратиться по ссылке: https://github.com/Raiffeisen-DGTL/cib-interns-test-task

Приложение написано на Spring Boot (MVC, Data JPA), Maven, JDK 17, в качестве базы данных — MySQL, для версионирования используется Flyway. 

Чтобы запустить приложение вместе с базой данных, потребуется docker-compose. Далее, нужно клонировать репозиторий и активировать скрипт
**start.sh**, наличие Мавена не обязательно (можно закоментировать соответствующие строки). Тесты выполняются в другой базе, которая запускается в отдельном контейнере командой **docker-compose -f docker-compose-test.yml up --build -d**.
