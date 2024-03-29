# Описание проекта

Выбор локации скважины для добывающей компании «ГлавРосГосНефть».

Предоставлены пробы нефти в трёх регионах: в каждом 10 000 месторождений, где измерили качество нефти и объём её запасов. 

## Задача

- Построить модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль.
- Проанализировать возможную прибыль и риски техникой Bootstrap.

- Шаги для выбора локации:
    - В избранном регионе ищут месторождения, для каждого определяют значения признаков;
    - Строят модель и оценивают объём запасов;
    - Выбирают месторождения с самым высокими оценками значений. Количество месторождений зависит от бюджета компании и стоимости разработки одной скважины;
    - Прибыль равна суммарной прибыли отобранных месторождений.
 
- Условия задачи:

    - При разведке региона исследуют 500 точек, из которых с помощью машинного обучения выбирают 200 лучших для разработки.
    - Бюджет на разработку скважин в регионе — 10 млрд рублей.
    - Доход с каждой единицы продукта составляет 450 тыс. рублей.
    - После оценки рисков нужно оставить лишь те регионы, в которых вероятность убытков меньше 2.5% т.е. вероятность получить 10 млрд рублей дохода с 200 лучших больше 95%, так как распределение двухстороннее.
    - Среди трех выбрать регион с наибольшей средней прибылью.

## Общий вывод

Техникой _Bootstrap_  перебраны 1000 комбинаций по 500 случайных скважин, из их числа отбирались 200 лучших (по объёму предсказанных запасов). На их примере расчитывалась возможная прибыль. Для оценки возможных значений прибыли был взят 95% доверительный интервал.

**Регион №2** имеет наибольшую _среднюю прибыль_ **456.05млн.**, и Вероятность убытков: **1.50%** - меньше допустимой (2.5%), следовательно регион подойдет для разработки, и является регионом для добычи нефти с наибольшей прибылью.

Таким образом можно сделать вывод что оценка рисков позволяет нам оставить только один регион под номером 2 в котором вероятность убытков 1.50% что меньше допустимого 2.5%.

