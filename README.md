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