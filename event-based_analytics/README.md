# Проект: [Событийная аналитика](event-based_analytics)

## Описание:
Мы работаем в стартапе, который продаёт продукты питания. 
Необходимо изучить воронку продаж, а также исследовать результаты A/A/B-эксперимента (изменение шрифтов во всём приложении)

## Основные шаги:
- чтение и предобработка датасетов
- исследовательский анализ данных
- анализ воронки событий
- анализ результатов эксперимента

## Стек: 
*pandas*, *numpy*, *matplotlib*, *scipy*, *datetime*, *plotly*

## Инструменты:
*jupyter notebook*

## В проекте даются выводы:
Было проврено 16 гипотез о равенстве долей пользователей, совершавших те или иные события воронки, из разных групп. 
Был выбран уровень значимости 0.05 с поправкой Бонферрони. 
Конечно, этот метод сильно уменьшает уровень значимости для каждого теста, но p-value во всех тестах был выше 0.05, 
поэтому в любом случае гипотезы не удалось бы опровергунть.

А/А-тест показал, что разбиение на группы работает корректно.
Ни одну из нулевых гипотез не удалось опровергнуть. Иными словами, изменение шрифтов в приложении не оказало значимого эффекта на поведение пользователей.
