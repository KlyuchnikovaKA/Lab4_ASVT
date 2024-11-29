Эта программа демонстрирует применение параллельного программирования для выполнения матричного умножения с использованием библиотеки MPI (Message Passing Interface).
Программа разбивает задачу на несколько процессов, что позволяет распределить вычисления и сделать их более эффективными.
Основные этапы программы:
1. Инициализация MPI: Создание MPI окружения и определение количества процессов и их рангов.
2. Инициализация данных: Главный процесс (с рангом 0) заполняет матрицы matrixA и matrixB и отправляет их другим процессам.
3. Вычисление: Каждый процесс вычисляет часть результирующей матрицы matrixC для своих закрепленных строк из matrixA и полной matrixB.
4. Сбор результатов: Главный процесс собирает части matrixC от всех процессов и выводит итоговую матрицу.
5. Вывод времени выполнения: После завершения всех вычислений и процесса сбора данные о времени выполнения выводятся на экран.
Вывод результатов программы:
![image](https://github.com/user-attachments/assets/a1291367-47a3-48aa-ae13-451e4c9007b8)

вывод в несколько потоков:
![image](https://github.com/user-attachments/assets/d39b9a51-7ff9-42e2-ae8d-e1209367f258)

![image](https://github.com/user-attachments/assets/51a5201a-3bf2-49c1-86a7-197a5a5eab69)
