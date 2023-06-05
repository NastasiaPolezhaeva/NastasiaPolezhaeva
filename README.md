# Портфолио: аналитик данных

##  Обо мне

Привет! Меня зовут Анастасия, я - начинающий аналитик.
Окончила Самарский медицинский университет по специальности "Лечебное дело". Прошла интернатуру и ординатуру по специальности "травматология и ортопедия". Работала 8 лет в клинической больнице.
Затем решила поменять вектор профессионального развития и в настоящий момент я завершаю обучение на платформе онлайн-университета skypro по специальности "Аналитик данных".
 
  В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практики
  
##  Навыки и технологии

-  Инструменты анализа данных: SQL, Excel
-  Языки программирования и библиотеки: Python, Pandas, math
-  Системы управления базами данных: MySQL, PostgreSQL
-  Средства визуализации данных: PowerBi

## Проекты

 ### Проект 1: Калькулятор юнит-экономики онлайн-школы
Что нужно было сделать:

>**Задача №1**. Настроить в калькуляторе учет корректировок планов маркетинга.
 
>**Задача №2**. Пересчитать план найма преподавателей.

Как решала:
1. *Добавила в список параметров калькулятора показатель "Поправочный коэффициент на привлечение".
Установила значение этого показателя по умолчанию, как 100% и добавила возможность изменять этот показатель через столбец "Изменение".
Настроила динамический расчёт количества новых студентов за период 05.21-04.22 с поправкой на этот коэффициент, т.е.в каждый месяц этого периода 
рассчётное значение количества новых студентов стало больше на 20%(с помощью функции ВПР притянула в таблицу план маркетинга по новым студентам 
и умножила на поправочный коэффициент).
Просчитала сценарий, при котором планы маркетинга будут увеличены на 12% при сохранении всех остальных настроек без изменений.*
2. *Добавила в калькулятор Найма преподавателей (Найм План) возможность изменять входные параметры: Пропускную способность П и Retention П - 
с помощью дополнительного столбца с процентными изменениями. Сделала поправку в расчёте общей пропускной способности (изменила формулу так,
чтобы отразить, что новые преподаватели в первый месяц своей работы могут проводить только половину уроков от средней пропускной способности
преподавателя, задаваемой параметром).  Обновила прогнозное количество уроков в соответствии с полученным количеством студентов из Задачи 1. 
Просчитала сценарий, при котором Пропускная способность П увеличится на 15 процентов, а Retention П упадёт на 2 процента. И, наконец, 
с помощью функции "Поиска решений" составила новый план найма с ограничением: за месяц нельзя нанять более 70 преподавателей.*

**Выводы(итоги)**:

**Итог №1**: Новое количество планируемых студентов с поправкой на коэфициент 12% (на листе Главный) и 
возможность корректировать план маркетинга.

**Итог №2**: Новый план найма преподавателей в соответствии с заданными условиями (на листе Найм План)

 ### Проект 2: Калькулятор юнит-экономики онлайн-кинотеатра

Что нужно было сделать:

>**Задача №1**. Посчитать юнит-экономику онлайн-кинотеатра, который работает по модели ежемесячной подписки.

>**Задача №2.** Предложить сценарий по настройке параметров для выхода на 25-процентную маржинальность.

Как решала: 

1.*Просчитала все фактические показатели необходимых метрик для юнит-калькулятора на основании имеющихся данных с апреля по август 2021г года. Ввела столбец "Планируемые показатели" и связала его со столбцом "Изменение", чтобы иметь возможность с помощью коэффициентов влиять на прогноз. С помощью исторических данных спрогнозировала все показатели на период с сентября 2021г по январь 2022г. Построила таблицу основных показателей "to be - as is".*

2.*С помощью функции "Поиска решений" и столбца "Изменение" настроила параметры с условием выхода маржинальности на 25 %.*

Ссылка на проект (ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)

**Выводы (итоги)**: Юнит-экономика продукта неэффективна и убыточна. Средняя маржинальность за период с мая по август 2021 года составила -90,45%. 
Количество новых подписок уменьшается. Retention падает. Высокие расходы на маркетинг ( почти 50%), высокие фиксированные расходы ( 47%).
Для выхода на получение 25-ти % маржинальности необходимо снизить средний CPA (он же CAC для нашего продукта) на 45%, повысить Retention не менее, чем на 7% и повысить стандартную цену подписки. 


### Проект 3: Когортный анализ онлайн-кинотеатра

Что нужно было сделать:

>**Задача №1**. Необходимо проанализировать клиентский LTV по когортам времени захода на платформу онлайн-кинотеатра и сделать выводы, какие когорты лучше, а какие хуже с точки зрения LTV

Как решала: 

*Построила сводную таблицу с абсолютными доходимостями клиентов по месячным когортам, а затем таблицу с клиентским Retention. На основании Retention рассчитала лайфтайм с помощью метода усредненных прямоугольников для каждой когорты. Рассчитала LTR для каждой когорты с помощью ARPU (предположила, что ARPU = 300). Рассчитала LTV с помощью усредненных костов для каждой когорты.*

Ссылка на проект (ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)

**Выводы (итоги)**: Распределение хороших и плохих когорт с точки зрения LTV.


### Проект 4: Построение витрины для модели машинного обучения в банке

Что нужно было сделать: 

>**Задача №1**. Написать скрипт, который сделает витрину со следующими полями:

- Внутренний идентификатор клиента — поле id_client.
- Название города — поле name_city из таблицы skybank.region_dict.
- Числовой признак, который принимает значение 1 для мужчин и 0 для женщин — новое поле nflag_gender на основании поля gender.
- Возраст — поле age.
- Числовая переменная, которая показывает, в первый ли раз клиент обратился к нам за кредитом, — поле first_time.
- Числовой признак, который принимает значение 1 при наличии мобильного телефона и 0 при его отсутствии — новое поле nflag_cellphone на основании поля cellphone.
- Числовая переменная, которая показывает, активен ли клиент, — поле is_active;
- Номер клиентского сегмента — поле cl_segm.
- Размер выданного кредита — поле amt_loan.
- Дата выдачи кредита — поле date_loan. Необходимо привести к формату даты.
- Тип выданного кредита — поле credit_type.
- Суммарный объем кредитов, выданных в этом городе.
- Доля данного кредита среди всех кредитов, выданных в этом городе.
- Суммарный объем кредитов, выданных в рамках указанного типа кредита.
- Доля данного кредита среди всех кредитов, выданных в рамках указанного типа кредита.
- Суммарный объем кредитов, выданных в рамках указанного типа кредита и города.
- Доля данного кредита среди всех кредитов, выданных в рамках указанного типа кредита и города.
- Количество кредитов, выданных в этом городе.
- Количество кредитов, выданных в рамках указанного типа кредита.
- Количество кредитов, выданных в рамках указанного типа кредита и города.

Как решала: 

*С помощью подзапроса вывела требуемые поля; суммы и количества посчитала с помощью оконных функций; последним этапом расчитала запрашивемые доли.* 

Ссылка на проект (ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)

**Выводы (итоги)**: Готовая витрина

### Проект 5: Моделирование изменения балансов студентов

Что нужно было сделать:

>**Задача №1** Посмотреть на изменения балансов студентов (на примере топ-1000 строк), собранных из CTE. Ответить на вопросы: 
Какие данные вас смущают? Какие вопросы стоит задавать дата-инженерам и владельцам таблиц?

>**Задача №2.** Создать визуализацию (линейную диаграмму) итогового результата. Какие выводы можно сделать из получившейся визуализации? 

Как решала: 

*Использовала конструкцию CTE. Узнала, когда была первая транзакция для каждого студента. Собрала таблицу с датами за каждый календарный день 2016 года. Узнала, за какие даты имеет смысл собирать баланс для каждого студента (даты после первой успешной транзакции). Нашла все изменения балансов, связанные с успешными транзакциями (нашла все транзакции и сгруппировала по юзеру и дате). Нашла баланс студентов, сформированный только транзакциями - куммулятивная сумма балансов транзакций. Посчитала количество пройденных за каждый день уроков для каждого ученика,а также куммулятивную сумму этих уроков для каждого ученика. Вычислила балансы каждого студента ( объединила куммулятивные суммы количества транзакций и количества уроков). Сделала выводы.*

Ссылка на проект (ссылка должна содержать демонстративные материалы: скриншоты, таблички, запросы, код. Работодатель должен иметь возможность быстро посмотреть результаты работы)

**Выводы**:

**Итог №1**: Вопросы к таблице Payments:
Почему в таблице о транзакциях имеются пустые строки в поле id_transaction?
Что значит status_name = created? созданный? Почему при отсутствии оплаты операции присвоен id_transaction?   

**Итог №2**: Выводы по визуализации: Онлайн-школа работает успешно, о чем говорит:
             <p>-рост кумулятивной суммы транзакций (на конец года составляет 21 798) <p>
              <p>-рост кумулятивной суммы транзакций (на конец года составляет 21 798) <p>
              <p>-рост баланса к концу 2016 года 4 126, то есть студенты продолжают покупать уроки на следующий год <p>
              <p>-опираясь на кривую sum_classes можно сделать вывод, что студенты предпочитают проходить уроки в будние дни, а в праздники и выходные наблюдается снижение количества проходимых уроков. <p>
             
## Контактная информация
Email: nastasya_polezhayeva@list.ru

