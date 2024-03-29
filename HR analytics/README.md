# Предсказание уровня удовлетворенности работой сотрудника и вероятности его увольнения

Компания предоставила данные с характеристиками сотрудников компании. Среди них — уровень удовлетворённости сотрудника работой в компании. Эту информацию получили из форм обратной связи: сотрудники заполняют тест-опросник, и по его результатам рассчитывается доля их удовлетворённости от 0 до 1, где 0 — совершенно неудовлетворён, 1 — полностью удовлетворён.

Задачами работы являлись:

- построить модель, которая сможет предсказать уровень удовлетворённости сотрудника на основе данных заказчика.
- построить модель, которая сможет на основе данных заказчика предсказать то, что сотрудник уволится из компании.
- 
1. Целевой признак для первой задачи — уровень удовлетворённости сотрудника работой в компании, моделирование необходимо выполнять методами регрессии.
2. Целевой признак для второй задачи - quit — увольнение сотрудника из компании, моделирование необходимо выполнять методами классификации.

Перед выполнением процесса моделирования были проведены: предобработка данных, исследовательский и корреляционный анализ признаков

Мало значимы для модели:

- Отдел, в котором работает сотрудник
- Наличие повышения


Сильнее всего влияют на целевой признак:

- Стаж сотрудника в этой компании
- Оценка руководителя
- Факт нарушения трудового договора
- Зарплата

В целевом признаке (quit) отмечен сильный дисбаланс классов. Дисбаланс классов объясняется спецификой задачи, так как факт увольнения фиксируется для небольшого процента покупателей. Нельзя устранить такой дисбаланс, не нарушив закономерности данных.


**Портрет уволившегося сотрудника:** Большинство из уволившихся сотрудников имеют уровень junior, и в основном имели небольшую и среднюю рабочую нагрузку. Никто из уволившихся сотрудников не получил премию за последний год работы, но при этом эти сотрудники довольно часто нарушали трудовой договор (каждый третий сотрудних в течении года). Распределение по отделам для работающих и уволившихся сотрудников схожее, поэтому поведение уволившегося сотрудника н зависит от отдела в котором он работает. Уволившиеся сотрудники получали средние оценки от руководителя 3 и 4, а также имели маленький стаж работы в компании до 3 лет. Уволившиеся сотрудники имели более низкую заработную плату.

**Рекомендация:** Бизнесу необходимо чаще обращать внимание на уровень удовлетворенности сотрудников уровня junior и чаще проводить оценку качества их работы и повышения. Молодые специалист не получают повышение и не довольны уровнем заработной платы, скорее всего факт нарушения трудового договора вызван имено недовльством сотрудников условиями работы. Уволившиеся сотрудники часто получали от руководитея оценку 4, что говорит о том, что в общем он был доволен работой сотрудника, поэтому компания теряет хорошие кадры, к тому же многие из уволившихся отработали в компании уже несколько лет.
