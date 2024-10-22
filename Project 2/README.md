# Анализ вакансий из HeadHunter (Блок 2. Подгрузка данных)

## Оглавление

1. Описание проекта
2. Какой кейс решаем?
3. Краткая информация о данных
4. Этапы работы над проектом
5. Результат
6. Выводы

### Описание проекта
Мы устроились на работу в кадровое агентство, которое подбирает вакансии для IT-специалистов. Наш первый проект — создание модели машинного обучения, которая будет рекомендовать вакансии клиентам агентства, претендующим на позицию Data Scientist. Сначала нам необходимо понять, что из себя представляют данные и насколько они соответствуют целям проекта. В литературе эта часть работы над ML-проектом называется Data Understanding, или анализ данных.



**Какой кейс решаем?**
Проект состоит из 4 частей, которые необходимо выполнять последовательно

**Этапы проекта::**

*знакомство с данными;
*предварительный анализ данных;
*детальный анализ вакансий;
*анализ работодателей;
*предметный анализ.

**Требования к оформлению ноутбука-решения**

* Решение оформляется только в Jupyter Notebook.
* Решение оформляется в соответствии с ноутбуком-шаблоном.
* Каждое задание выполняется в отдельной ячейке, выделенной под задание (в шаблоне они помечены как ваш код здесь). Не следует создавать много ячеек для решения задачи — это провоцирует неудобства при проверке.
* Текст SQL-запросов и код на Python должны быть читаемыми. Не забывайте про отступы в SQL-коде.
* Выводы по каждому этапу оформляются в формате Markdown в отдельной ячейке (в шаблоне они помечены как ваши выводы здесь).
* Выводы можно дополнительно проиллюстрировать с помощью графиков. Они оформляются в соответствии с теми правилами, которые мы приводили в модуле по визуализации данных.
* Удалить ячейку с данными соединения перед фиксацией работы в GitHub.

### Формат ноутбука с решением:

Номер задания.
Код для получения ответа.
Результат запроса.
Выводы по блоку заданий.
Общий вывод в конце по результатам анализа, имеющихся данных по вакансиям.
Критерии оценки (максимум 8 баллов):


### Что практикуем

Учимся писать хороший код на Python;
Учимся работать с pgSQL;
Учимся получать по запросу нужные данные для минимальной следующей обработки;
Размещаем итог на GitHub;
Краткая информация о данных;

**Исходные данные**

VACANCIES (таблица со следующими столбцами):
*AREAS Таблица-справочник, которая хранит код города и его название.
*EMPLOYERS Таблица-справочник со списком работодателей.
*INDUSTRIES Таблица-справочник вариантов сфер деятельности работодателей.
*EMPLOYERS_INDUSTRIES Дополнительная таблица, которая существует для организации связи между работодателями и сферами их деятельности.


### Этапы работы над проектом

Подготовка данных;
Решение заданий
Составление графиков;
Выводы.


#### Результат:
*Проведен анализ полученных данных;
*Подготовлена и выведена информация для последующих выводов;
*Подготовлена визуализация анализируемых данных;
*Сделаны выводы и предложения.


Выводы:
Спрос на специалистов в DS велик, заработная плата сравнительно высока, но нужно обладать довольно большим числом навыков. Заработная плата довольно резко растет с опытом. Сложности для модели - отсутствие указанной заработной платы, сфер деятельности, региона работодателя.