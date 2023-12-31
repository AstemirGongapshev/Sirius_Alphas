Управление Финансовыми Портфелями

## Описание

Этот проект предоставляет инфраструктуру и примеры для разработки и тестирования алгоритмических торговых стратегий (АТС).
Включает в себя библиотеку функций для анализа и оценки стратегий, а также набор альф и портфельных стратегий для демонстрации возможностей.

## Файлы в Репозитории

### `help_functions.py`

# Библиотека Функций для АТС

## Описание

Библиотека предоставляет набор инструментов для анализа и выполнения алгоритмических торговых стратегий. Функции позволяют выполнять расчеты ключевых метрик, 
обработку данных и управление портфелями.

## Функции Библиотеки

- `truncate`: Усечение данных для управления уровнем риска или для сокращения выбросов в наборе данных.
- `neutralize`: Нейтрализация определенных рыночных факторов в альфа-сигналах для создания стратегий, не зависящих от этих факторов.
- `normalize`: Нормализация данных или сигналов для обеспечения сопоставимости между различными источниками.
- `prof`: Подсчет доходности альфы или портфеля на основе временного ряда цен или доходностей.
- `ret_matrix`: Создание матрицы доходностей для различных инструментов или альф.
- `volatility`: Расчет волатильности альфы или портфеля для оценки риска.
- `turnover`: Вычисление оборота альфы, что важно для оценки торговых издержек.
- `cut_middle`: Функция для усечения центральной части распределения, фокусируясь на крайних значениях.
- `cut_outliers`: Удаление или ограничение влияния выбросов в данных для уменьшения искажения модели.
- `corr`: Расчет корреляции между двумя альфами для оценки их взаимосвязи и уникальности.
- `rank_vector`: Ранжирование данных или сигналов, превращение их в порядковые значения для создания ранжированных стратегий.
- `decay`: Применение функции замедления для сглаживания временных рядов и уменьшения оборота.
- `sharpe`: Вычисление коэффициента Шарпа для оценки относительной привлекательности альфы или стратегии.
- `max_drawdown`: Расчет максимальной просадки для определения потенциального максимального убытка стратегии.
- `cumupnl`: Вычисление накопленной прибыли (cumulative PnL) для измерения общей эффективности стратегии.

Каждая функция включена для оптимизации процесса создания и оценки АТС.


### `main.py`

Этот файл демонстрирует применение функций из `help_functions.py` на примере 10 альф (альфа-сигналов) и 3 портфельных стратегий.

Примеры альф:
- `alpha_1`, `alpha_2`, ..., `alpha_10`: Описание того, что каждая альфа представляет и как она может быть использована в стратегии.

Примеры портфельных стратегий:
- `portfolio_1`, `portfolio_2`, `portfolio_3`: Комбинации альфа-сигналов и методы их взвешивания для создания диверсифицированного портфеля.


