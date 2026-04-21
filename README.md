# commit-day-classifier
Binary classification of day type from commit activity

Описание:
Модель предсказывает тип дня — **рабочий** или **выходной** — на основе временных меток коммитов.

Используемые методы
- Feature Engineering: создание признаков `am` (коммиты до полудня) и `pm` (после полудня)
- Масштабирование признаков (`StandardScaler`)
- Модели: LogisticRegression, SVC, DecisionTreeClassifier
- Визуализация границ решений (`DecisionBoundaryDisplay`) и plot_tree

Результаты:
Наивное предсказание (всегда working_day) даёт точность 0.714286. Все обученные модели превосходят этот базовый уровень, а дерево решений достигает почти 95% точности.
