## Определение возраста покупателей магазина по фотографии

**Описание проекта:**
Сетевой супермаркет «Хлеб-Соль» внедряет систему компьютерного зрения для обработки фотографий покупателей. 

**Описание датесетов:**
Набор из 7591 фотографий людей с указанием возраста.

**Задачи бизнеса в этом проекте:**
1. Анализировать покупки и предлагать товары, которые могут заинтересовать покупателей этой возрастной группы;
1. Контролировать добросовестность кассиров при продаже алкоголя.

**Инструменты и навыки:**  
keras, ResNet50, `numpy`, `pandas`, `sklearn`

**Выводы:**  
Модель обучалась в течение 10 эпох батчами по 32 фотографии и **достигла MAE = 5,87 лет** на валидационной (и на тестовой) выборках. Время обучения - около 6,5 минут.
Ошибка в 6 лет некритична для рекомендаций товаров по возрастной группе, так что первая задача достигнута.
Вторая задача более сложная и строгая. Учитывая размер ошибки, можем доверять решению модели, когда она даёт оценку человеку 24 и более лет - тогда с высокой вероятностью покупателю уже есть 18 лет.

__[Дополнительный вариант просмотра тетрадки](https://nbviewer.jupyter.org/github/artdaal/yandex-practicum-projects/blob/main/14_computer_vision/CV.ipynb)__