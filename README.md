# Анализ данных из базы данных

Этот проект представляет собой анализ данных из базы данных, включающий предобработку данных, исследовательский анализ данных (EDA) и проверку гипотез. В проекте используются данные из двух таблиц: `doc_views.csv` и `payments.xlsx`.

## Структура проекта

1. **Импорт библиотек**: В проекте используются библиотеки `pandas`, `numpy`, `matplotlib` и `hashlib` для обработки данных, визуализации и хеширования.

2. **Загрузка данных**: Данные загружаются из файлов `doc_views.csv` и `payments.xlsx`. В таблице `doc_views` содержатся данные о просмотрах документов, а в таблице `payments` — данные о платежах.

3. **Предобработка данных**:
   - **Переименование полей**: Некоторые столбцы в таблице `doc_views` переименованы для удобства.
   - **Преобразование типов данных**: Преобразование данных в столбцах `viewed_at` и `passport_number` в таблице `doc_views`.
   - **Обработка пропусков**: Удаление строк с пропущенными значениями в таблице `payments` и заполнение пропущенных значений в таблице `doc_views`.
   - **Анонимизация данных**: Хеширование данных в столбце `passport_number` для анонимизации.

4. **Исследовательский анализ данных (EDA)**:
   - **Локация покупателей**: Анализ локаций покупателей и сумм платежей.
   - **Влияние пробных периодов на платежи**: Проверка гипотезы о том, что пробные периоды влияют на последующие платежи.

5. **Загрузка данных в ChatGPT**: Данные экспортируются в файлы `doc_views_result.csv` и `payments_result.csv` для дальнейшего анализа.

6. **Генерация гипотез и проверка**:
   - **Гипотеза о пробных периодах**: Проверка гипотезы о том, что пользователи, прошедшие пробный период, чаще совершают покупки. Результат показал, что 7.4% пользователей, совершивших покупку, ранее использовали пробный период.

## Использование

Для запуска проекта необходимо установить необходимые библиотеки:

```bash
pip install pandas numpy matplotlib
```
***Затем можно запустить Jupyter Notebook и открыть файл AnalisysDataBase.ipynb для выполнения анализа***
## Файлы
- **doc_views.csv:** Данные о просмотрах документов.

- **payments.xlsx:** Данные о платежах.

- **doc_views_result.csv:** Результаты обработки данных о просмотрах документов.

- **payments_result.csv:** Результаты обработки данных о платежах.

## Автор
Проект выполнен в рамках курса по анализу данных
```
Этот файл `README.md` предоставляет общее описание проекта, его структуры, используемых данных и результатов анализа. Вы можете дополнить его информацией о себе и ссылками на другие ресурсы, если это необходимо.
```

