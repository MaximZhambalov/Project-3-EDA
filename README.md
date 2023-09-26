![](./images/logo.jpg)
# <center> Проект 3: Прогнозирование рейтинга отеля на Booking </center>

## Оглавление
1. [Описание проекта](#Описание-проекта)
2. [Описание данных](#Описание-данных)
3. [Зависимости](#Зависимости)
4. [Установка проекта](#Установка-проекта)
5. [Использование проекта](#Использование-проекта)
6. [Выводы](Использование-проекта)

## Описание проекта

**Данный проект** выполнен с целью научиться обрабатывать исходные данные, готовить их к использованию в модели, а также узнать что такое Kaggle и с чем его едят :)

**О структуре проекта:**
* [images](./images) - папка с изображениями, необходимыми для проекта.
* [data](./data) - папка с датасетом.
* [catboost_info](./catboost_info) - папка со служебными данными модели (я использую CatBoost от Yandex)
* [EDA_Project_3_model_FINAL.ipynb](./EDA_Project_3_model_FINAL.ipynb) - jupyter-ноутбук, содержащий основной код проекта: SQL-запросы и обработка этих запросов, а также выводы из полученных данных.


## Описание данных
Представьте, что вы работаете дата-сайентистом в компании *Booking*. Одна из проблем компании — это нечестные отели, которые накручивают себе рейтинг. Одним из способов обнаружения таких отелей 
является построение модели, которая предсказывает рейтинг отеля. Если предсказания модели сильно отличаются от фактического результата, то, возможно, отель ведёт себя нечестно, и его стоит проверить.

## Используемые зависимости
* Python (3.9):
    * [pandas (1.3.4)](https://pandas.pydata.org)
    * [numpy (1.23.5)](https://pypi.org/project/psycopg2/)
    * [seaborn (0.12.2)](https://plotly.com/python/)
    * [matplotlib (3.6.3)](https://matplotlib.org/)
    * [scikit-learn (1.2.2)](https://scikit-learn.org/stable/index.html)
    * [category-encoders (2.6.1)](https://contrib.scikit-learn.org/category_encoders/)
    * [catboost (1.2)](https://catboost.ai/)
    * [pycountry-convert (0.7.2)](https://pypi.org/project/pycountry-convert/)
    * [afinn 0.1](https://pypi.org/project/afinn/)

## Установка проекта
```
git clone https://github.com/MaximZhambalov/HeadHunter_Project_2
```
Датасет по проекту можно найти [здесь](https://www.kaggle.com/competitions/sf-booking/data)

## Использование
Вся информация о работе представлена в jupyter-ноутбуке EDA_Project_3_model_FINAL.ipynb.

## Выводы
В этом проекте:
- проведён разведовательный анализ данных, обработан и подготовлен датасет для модели;
- была построена модель, предсказывающая рейтинг отеля. Финальное значение метрики (MAPE) - 12.5%.