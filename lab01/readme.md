### Результаты метрик

#### Классификация

| Модель                      | AUPRC | Average Precision | Precision | Recall |
|-----------------------------|-------|-------------------|-----------|--------|
| scikit-learn до оптимизации | 0.050 | 0.002             | 0.002     | 0.312  |
| scikit-learn после оптимизации | 0.508 | 0.337             | 0.311     | 0.667  |
| Собственная реализация до оптимизации | 0.050 | -                 | 0.00      | 0.00   |
| Собственная реализация после оптимизации | 0.490 | -                 | 0.60      | 0.80   |

#### Регрессия

| Модель                      | MAE     | MSE        | RMSE     | R²       |
|-----------------------------|---------|------------|----------|----------|
| scikit-learn до оптимизации | 226.435 | 573041.413 | 756.995  | 0.142667 |
| scikit-learn после оптимизации | 245.803 | 165005.640 | 406.209  | 0.043023 |
| Собственная реализация до оптимизации | 245.803 | 165005.640 | 406.209  | 0.043023 |
| Собственная реализация после оптимизации | 263.118 | 162683.469 | 403.340  | 0.056491 |

### Краткий вывод

Оптимизация классификационной модели с использованием scikit-learn дала значительные улучшения во всех метриках, повысив способность модели точно определять положительные классы. Собственная реализация также продемонстрировала успешную оптимизацию, несмотря на отсутствие начальных результатов.

Однако оптимизация модели регрессии привела к ухудшению показателей как для scikit-learn, так и для собственной реализации. Это подчеркивает необходимость дальнейшего анализа и настройки гиперпараметров, а также возможного применения дополнительных методов обработки данных или изменения архитектуры модели.