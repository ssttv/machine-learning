# machine-learning
0. Interactive grouping. - пример ООП.

Модуль combiner.py реализует аналог блока "Interactive grouping" из SAS Miner, включая графический интерфейс.
В git выложена версия с усеченной функциональностью, позволяющая работать исключительно с категориальными признаками и заменяющая значения признаков метками групп вместо woe. Написан для python 3.6.1.

"Группинг" используется в задачах классификации. Для катеогориальных признаков "группинг" сводится к замене группы значениий признака одним. 

Все множество объектов обучающей выборки делится категориальным признаком на непересекающиеся подмножетсва, объекты каждого из подмножеств обладают своим значением признака. Для каждого подмножества можно определить долю объектов целевого класса в этом подмножетсве и доверительный интервал на эту долю. Подмножетсва с пересекающимися доверительными интервалами объединяются. Новый, производный, категориальный признак получается путем замены значений, выделяющих объединеные подмножетсва, одной меткой. 

"Группинг" напоминает построение неглубокого дерева решений на категориальном признаке с присвоением каждому листу построенного дерева отдельной метки.  

 <b> NN for Time Series </b>

Применение полносвязной нейронной сети прямого распростанения для прогнозирования большого количества (~6000 тыс.) временных рядов нагрузки на сотрудников отделеный банка. Применение данного подхода позволило доститчь более высокого качетсва прогноза (~15% по MAE),  кратно сократить время обучения и примененния модели, по сравнению с подходом предполагавшем обучение SARIMAX c экзогенными признаками для каждого ряда в отдельности.  

1. Churn prediction - смотрите пояснительную записку. 

В представленной работе описан процесс создания классификатора для конкретного  эмипирческого материала –  40 тысяч клиентов French Telecom company Orange – одного из мировых лидеров в области телекоммуникационных услуг (более 170 млн. пользователей). Рассмотрены различные методы предобработки данных и отбора значимых признаков. Оценено влияние предобработки на качество линейных методов классификации,  «случайного леса», градиентного бустинга над решающими деревьями. Опробован «stacking»-подход к решению задачи. Проведен расчет экономического эффекта от применения разработанной модели.
Программная реализация алгоритмов обработки и классификации выполнена на языке Python 2.7 в интерактивной оболочке Jupyter Notebook c использованием библиотек pandas, skipy, sklearn, seaborn. 

2. Credit score

Проверка различных статистических гипотез на выборке заемщиков допустивших дефолт по кредиту. 

3. Time series analysis

Прогнозирование ряда средней заработной платы в России.
SARIMAX

4. Sentiment analysis

Анализа тональности отзывов на фильмы из стандартного датасета nltk.

5. Simple clustering

PCA + DBSCAN

6. Choice of banner

На прошедшей неделе в рекламной сети параллельно размещалось два баннера. Оба баннера были показаны один миллион раз. Первый получил 10 000 кликов и 500 установок, а второй — 10 500 кликов и 440 установок. Какой баннер оставить, а какой отключить? 

7. Fraud on road

Анализ выборки страховых событий (ДТП с двумя участниками) на возможное мошенничество. Выделение тех клиентов, относительно которых существует подозрение на мошеннические действия.

8. Simple client-server

asyncio, python3

9. SQL with python

Два простых запроса. 

10. Working with logs

Имеется файл log.txt размером 1Tb, содержащий лог в следующем формате: номер записи, тип запроса, время отклика. 
Напишите на Python программу, которая для каждого типа запроса подсчитывает среднее время отклика и 95% доверительный интервал для этой величины.
