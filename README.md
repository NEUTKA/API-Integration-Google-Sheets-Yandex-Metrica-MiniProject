# Мини-проект: Анализ поведения пользователей на сайте Яндекс.Метрики с использованием API

## Описание

В этом мини-проекте мы работаем с демо-данными Яндекс.Метрики, анализируя поведение пользователей на сайте за последнюю неделю. Используем уже выгруженные данные для анализа посещений, чтобы можно было повторить шаги без необходимости обращения к реальному API. Однако каждый запрос также можно выполнить к настоящему API для тренировки. Задачи включают анализ источников трафика, поведения ботов и людей, а также работу с Google SpreadSheets и VK API для автоматизации отправки данных.

## Задачи

1. **Анализ распределения посещений по типам пользователей**
   - Постройте график распределения количества посещений от ботов и обычных пользователей Яндекс.Метрики по дням.
   
2. **Определение посещений с браузера Google Chrome**
   - Определите процент посещений сайта с браузера Google Chrome от общего числа посещений.

3. **Анализ доли ботов по браузерам**
   - Выясните, с какого браузера приходит наибольший процент ботов от общего числа посещений с этого браузера.

4. **Расчёт метрики доли заходов по типам пользователей и браузерам**
   - Выгрузите данные, содержащие информацию о дне, типе пользователя и браузере.
   - Создайте новую колонку, в которой рассчитывается доля заходов на сайт для каждой комбинации день/тип пользователя/браузер.
   - Укажите процент заходов реальных пользователей через браузер Safari с точностью до одного знака после запятой.

5. **Отправка данных в Google SpreadSheet и сообщение через VK API**
   - Сохраните данные из предыдущего шага в Google SpreadSheet с помощью библиотеки `gspread`.
   - С помощью VK API отправьте себе ссылку на таблицу в личные сообщения ВКонтакте (не забудьте открыть доступ к файлу).

6. **Объединение данных с другим аналитиком и расчет визитов**
   - Прочитайте дополнительные данные из Google SpreadSheet и объедините их с таблицей из предыдущего шага.
   - В объединенной таблице рассчитайте количество визитов на уникального пользователя в разрезе по браузеру и типу пользователей (боты/люди).
   - Укажите количество визитов на одного пользователя для ботов, заходящих с браузера Google Chrome, округлите до целого.

## Данные

### Датасеты, используемые в проекте:
- **Данные Яндекс.Метрики** — включает информацию о посетителях сайта за неделю.
- **Данные Google SpreadSheet** — данные о посещениях, сгенерированные другим аналитиком для совместной обработки.

#### Основные колонки в данных Яндекс.Метрики:
- **date**: Дата
- **user_type**: Тип пользователя (бот/человек)
- **browser**: Браузер, используемый для захода
- **visits**: Количество визитов
- **users**: Уникальные пользователи
- **platform**: Платформа

## Выводы

Мини-проект показал, как применять API для работы с внешними сервисами и обмена данными, от Google SpreadSheets до VK API. Также были рассмотрены методы анализа данных посещений и их распределения по типам пользователей, браузерам и платформам, что может быть полезно в задачах по анализу пользовательского поведения и выявления ботов.


# Mini-Project: User Behavior Analysis on Yandex.Metrica Website Using API

## Description

In this mini-project, we work with demo data from Yandex.Metrica, analyzing user behavior on a website over the past week. We use already exported data for analysis so that the steps can be repeated without the need for real API calls. However, each request can also be made to the actual API for practice. Tasks include traffic source analysis, bot and human behavior analysis, and working with Google Spreadsheets and VK API for automating data sending.

## Tasks

1. **Analysis of Visits by User Types**
   - Create a chart showing the distribution of visits by bots and regular users of Yandex.Metrica across different days.

2. **Determining Visits from Google Chrome Browser**
   - Calculate the percentage of visits from Google Chrome browser out of the total number of visits.

3. **Bot Share Analysis by Browser**
   - Identify which browser has the highest percentage of bot visits out of the total visits for that browser.

4. **Calculation of Visit Share by User Type and Browser**
   - Load data containing information about the date, user type, and browser.
   - Create a new column where you calculate the visit share for each combination of day/user type/browser.
   - Provide the percentage of visits from real users using the Safari browser with one decimal point of precision.

5. **Sending Data to Google Spreadsheet and VK API Message**
   - Save the data from the previous step to a Google Spreadsheet using the `gspread` library.
   - Send the link to the spreadsheet to yourself via VK API (remember to open access to the file).

6. **Merging Data with Another Analyst and Calculating Visits**
   - Read additional data from Google Spreadsheet and merge it with the table from the previous step.
   - In the merged table, calculate the number of visits per unique user, broken down by browser and user type (bots/people).
   - Provide the number of visits per user for bots visiting from the Google Chrome browser, rounded to the nearest whole number.

## Data

### Datasets Used in the Project:
- **Yandex.Metrica Data** — includes information on website visitors for the past week.
- **Google Spreadsheet Data** — data about visits, generated by another analyst for joint processing.

#### Main Columns in Yandex.Metrica Data:
- **date**: Date
- **user_type**: User type (bot/human)
- **browser**: Browser used for visiting the site
- **visits**: Number of visits
- **users**: Unique users
- **platform**: Platform

## Conclusions

The mini-project demonstrated how to use APIs for working with external services and exchanging data, from Google Spreadsheets to VK API. It also explored methods for analyzing visit data and its distribution by user types, browsers, and platforms, which can be valuable in tasks related to user behavior analysis and bot detection.