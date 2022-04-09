## Рекомендательная модель для телеком-компании

**Описание проекта:**
В распоряжении предобработанный датасес с данными о поведении клиентов.
Датасет содержит такие признаки, как: используемый пользователем тариф, ежемесячные расходы разных услуг (минуты разговора, количество сообщенийи интернет-трафика).


**Задачи проекта:** 
Построить модель для задачи классификации, которая выберет подходящий тариф. Модель оценивается метрикой accuracy, нужно довести до значения 0.75 на тестовой выборке.

**Инструменты и навыки:**  
машинное обучение, классификация, визуализация данных, `pandas`, `sklearn`, `Matplotlib`, `Seaborn`, `numpy`, `scipy`

**Выводы:**  
В текущей задаче классификации были обучены и сравнены 4 различных модели: дерево решений, случайный лес, метод k-ближайших соседей и логистическая регрессия.
Для подбора гиперпараметров моделей использовали 5-кратную K-fold кросс-валидацию. 
Наилучший результат показал алгоритм **Случайный лес** с accuracy=0.813

__Дополнительный вариант просмотра тетрадки [тут](https://nbviewer.jupyter.org/github/artdaal/yandex-practicum-projects/blob/main/06_basic_ML/Model_for_tariff_recommendation.ipynb)__