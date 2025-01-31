# Принятие решений в бизнесе

[Ссылка на проект](https://github.com/runinred/Practicum_projects/blob/main/AB-test%20review/AB-test%20review.ipynb)

## Описание проекта

Цель исследования: проверка гипотез и анализ выводов. В рамках проекта необходимо осуществить следующие основные задачи: приоритизация гипотез; запуск A/B-тестов; анализ результатов.



## Навыки и инструменты

- **python**
- **pandas**
- **matplotlib**
- **seaborn**
- **scipy**
- **ICE**
- **RICE**
- **A/B tests**




## Вывод

На «сырых» данных:
- отказ от основной гипотезы в пользу альтернативной гипотезы, т.к. имеются статистически значимые различия в среднем количестве заказов между группами; выигрыш группы В составляет 13,8%;
- основную гипотезу не отвергаем, т.к. статистически значимых различий в среднем чеке нет, хотя выигрыш группы В по среднему чеку составляет 25,9%, такое значение могло получиться под влиянием аномальных сумм заказов, то есть выбросов.

На «очищенных» данных:
- отказ от основной гипотезы в пользу альтернативной гипотезы, т.к. имеются статистически значимые различия в среднем количестве заказов между группами, выигрыш группы В составляет 16,7%;
- основную гипотезу не отвергаем, т.к. статистически значимых различий в среднем чеке нет, хотя проигрыш группы В по среднему чеку составляет 7.5%.

После очистки от аномальных значений, оценка гипотез не изменилась, а результаты отношений претерпели значительные изменения.
Были выявлены аномально большие заказы, в частности заказ на сумму более 1,294 млн.

Проведение теста рекомендуется остановить, поскольку по результатам тестирования - группа В показала себя значительно более эффективной, с выигрышем в 16,7% в части среднего количества заказов на посетителя. Таким образом, на каждого посетителя из группы В приходится на 16.7% больше заказов, чем на каждого посетителя из группы А, что может увеличить общую выручку относительно посетителей из группы В.

