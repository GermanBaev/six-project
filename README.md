# six-project
**Постановка задачи:**

В данном проекте было необходимо спрогнозировать, уйдёт ли клиент из банка в ближайшее время или нет. 
В распоряжении исторические данные о поведении клиентов и расторжении договоров с банком. 
Нужно было построить модель с предельно большим значением F1-меры. Чтобы точность модели удовлетворяла заказчика, следовало довести метрику до 0.59.
Дополнительно измерялась AUC-ROC и сравнивалась со значением F1-меры.

**Используемые модели:**

В данном проекте использовались модели решающего дерева, случайного леса и логистической регрессии. Плюс применялись техники борьбы с дисбалансом классов.

**Результат применения моделей:**

Наилучшие результаты получились у комбинации ***модели случайного леса*** и ***техники изменения порога классификации + взвешивания классов*** на валидационной и тестовой выборках:

| Выборка | F1-мера | ROC-AUC |
| :- | :- | :- |
| Валидационная | 0.6595059076262083 | 0.8692827291933104 |
| Тестовая | 0.6053921568627452 | 0.8549638462675583 |
