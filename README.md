# 09-ci-01-intro

# Домашнее задание к занятию 7 «Жизненный цикл ПО»

## Подготовка к выполнению

1. Получить бесплатную версию Jira - https://www.atlassian.com/ru/software/jira/work-management/free (скопируйте ссылку в адресную строку). Вы можете воспользоваться любым(в том числе бесплатным vpn сервисом) если сайт у вас недоступен. Кроме того вы можете скачать [docker образ](https://hub.docker.com/r/atlassian/jira-software/#) и запустить на своем хосте self-managed версию jira.
2. Настроить её для своей команды разработки.
3. Создать доски Kanban и Scrum.
4. [Дополнительные инструкции от разработчика Jira](https://support.atlassian.com/jira-cloud-administration/docs/import-and-export-issue-workflows/).

## Основная часть

Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить жизненный цикл:

1. Open -> On reproduce.
2. On reproduce -> Open, Done reproduce.
3. Done reproduce -> On fix.
4. On fix -> On reproduce, Done fix.
5. Done fix -> On test.
6. On test -> On fix, Done.
7. Done -> Closed, Open.

Остальные задачи должны проходить по упрощённому workflow:

1. Open -> On develop.
2. On develop -> Open, Done develop.
3. Done develop -> On test.
4. On test -> On develop, Done.
5. Done -> Closed, Open.

**Что нужно сделать**

1. Создайте задачу с типом bug, попытайтесь провести его по всему workflow до Done. 
2. Создайте задачу с типом epic, к ней привяжите несколько задач с типом task, проведите их по всему workflow до Done. 
3. При проведении обеих задач по статусам используйте kanban. 
4. Верните задачи в статус Open.
5. Перейдите в Scrum, запланируйте новый спринт, состоящий из задач эпика и одного бага, стартуйте спринт, проведите задачи до состояния Closed. Закройте спринт.
6. Если всё отработалось в рамках ожидания — выгрузите схемы workflow для импорта в XML. Файлы с workflow и скриншоты workflow приложите к решению задания.

---

### Как оформить решение задания

Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.

---
Попробовал создать несколько багов
Тасков и привязать к Epic
В Scrum не сразу понял, что нужно задачу перевести в статус (дополнить скриншот)


![Снимок экрана 2025-07-30 в 22.14.30.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.14.30.png)
![Снимок экрана 2025-07-30 в 22.14.42.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.14.42.png)
![Снимок экрана 2025-07-30 в 22.19.38.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.19.38.png)
![Снимок экрана 2025-07-30 в 22.20.30.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.20.30.png)
![Снимок экрана 2025-07-30 в 22.23.03.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.23.03.png)
![Снимок экрана 2025-07-30 в 22.25.16.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.25.16.png)
![Снимок экрана 2025-07-30 в 22.27.19.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.27.19.png)
![Снимок экрана 2025-07-30 в 22.29.52.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.29.52.png)
![Снимок экрана 2025-07-30 в 22.30.05.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.30.05.png)
![Снимок экрана 2025-07-30 в 22.30.21.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.30.21.png)
![Снимок экрана 2025-07-30 в 22.30.36.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.30.36.png)
![Снимок экрана 2025-07-30 в 22.30.44.png](https://github.com/Werest/09-ci-01-intro/blob/097834f263a7d203236a84125c3599a53f5abf42/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%202025-07-30%20%D0%B2%2022.30.44.png)