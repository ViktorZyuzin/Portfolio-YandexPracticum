# Описание проекта

Оператор мобильной связи **«Мегалайн»** выяснил: многие клиенты пользуются архивными тарифами. Компания желает построить систему, способную проанализировать поведение клиентов и предложить пользователям новый тариф: _«Smart»_ или _«Ultra»_.

В распоряжении данные о поведении клиентов, которые уже перешли на эти тарифы. Нужно построить модель для задачи классификации, которая выберет подходящий тариф.

Построить модель с максимально большим значением accuracy минимум 0.75. Проверить accuracy на тестовой выборке.

## Итоговый вывод
- В ходе исследования удалось построить модель с максимально большим значением accuracy для классификации целевого признака - подбор тарифа мобильного пользователя.

- Выбор состоял из трех моделей по алгоритмам классификации: дерево решений. случайный лес и логистическая регрессия.

- Лучшей стала модель на алгоритме случайного леса с глубиной: 9 и числом деревьев: 20.

- Доля правильных ответов на тестовой выборке достигла 0.805.
