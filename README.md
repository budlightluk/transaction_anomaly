Генерация синтетических данных транзакций и обнаружение аномалий
Этот проект создает синтетические данные транзакций и применяет алгоритм Local Outlier Factor (LOF) для обнаружения аномалий. Основные этапы включают генерацию данных, предварительную обработку, масштабирование, обнаружение аномалий и детализированную визуализацию результатов.

Обзор
Цель проекта - создать реалистичный синтетический набор данных финансовых транзакций и выявить потенциальные аномалии с использованием методов машинного обучения. Процесс включает в себя генерацию транзакций с различными атрибутами, масштабирование данных, применение алгоритма LOF для обнаружения аномалий и профессиональную визуализацию результатов.

Этапы
1. Генерация данных
Функция генерации синтетических данных создает набор данных со следующими атрибутами:

Customer ID (ID клиента): Уникальный идентификатор для каждого клиента.
Merchant ID (ID продавца): Уникальный идентификатор для каждого продавца.
Transaction Amount (Сумма транзакции): Сумма каждой транзакции, следующая логнормальному распределению.
Transaction Date (Дата транзакции): Случайным образом выбранные даты между 2010 и 2020 годами.
Transaction Category (Категория транзакции): Категория транзакции (например, Еда, Электроника).
Transaction Type (Тип транзакции): Тип транзакции (например, Кредит, Дебет).
2. Загрузка данных
Сгенерированные данные сохраняются в CSV-файл, а затем загружаются для дальнейшей обработки.

3. Предварительная обработка данных
Масштабирование: Только числовые столбцы масштабируются с использованием StandardScaler для стандартизации данных.
4. Обнаружение аномалий
Алгоритм LOF: Алгоритм Local Outlier Factor применяется к масштабированным данным для обнаружения аномалий. Алгоритм вычисляет аномальные оценки для каждой транзакции, указывая степень их отклонения от нормы.
5. Визуализация
Предоставляются три ключевых визуализации для анализа результатов:

Гистограмма аномальных оценок: Показывает распределение аномальных оценок с KDE для более плавного представления.
Точечный график: Отображает зависимость между Суммой транзакции и ID клиента, с точками, окрашенными по аномальным оценкам.
Парный график: Визуализирует парные отношения между числовыми признаками (ID клиента, ID продавца, Сумма транзакции), окрашенными по аномальным оценкам.
Результаты
Визуализации помогают понять распределение аномальных оценок и выявить потенциальные отклонения в данных транзакций. Эти инсайты могут быть полезны для дальнейшего анализа и разработки стратегий по обработке аномальных транзакций.

Заключение
Этот проект предоставляет комплексный подход к генерации синтетических данных транзакций и применению методов обнаружения аномалий. Детализированные визуализации улучшают понимание результатов и облегчают передачу полученных выводов.

Danila Ladygin
budlighterluk@gmail.com
@SkyWalker_OG
