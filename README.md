# Лабораторная работа(3): Анализ и сравнение функций активации в нейронных сетях для задач классификации

Этот репозиторий содержит пример использования различных функций активации в нейронных сетях для классификации рукописных цифр с использованием датасета MNIST.

## Обзор

Цель этого проекта - продемонстрировать влияние различных функций активации на процесс обучения и производительность нейронных сетей. Для обучения и оценки используется датасет MNIST, содержащий изображения цифр от 0 до 9.

## Модели

Реализованы несколько моделей, каждая из которых использует различную функцию активации:

- Сигмоида
- Гиперболический тангенс (Tanh)
- Rectified Linear Unit (ReLU)
- Leaky Rectified Linear Unit (Leaky ReLU)
- Parametric Rectified Linear Unit (PReLU)
- Gaussian Error Linear Unit (GELU)

Каждая модель компилируется с оптимизатором Adam, функцией потерь categorical crossentropy и метрикой accuracy.

## Обучение

Модели обучаются на тренировочном датасете MNIST с размером пакета 64 в течение 10 эпох. Процесс обучения визуализируется графиками потерь и точности для тренировочного и валидационного наборов данных.

## Структура файлов

- `main.py`: Основной скрипт с определением моделей, обучением и оценкой.
- `utils.py`: Вспомогательные функции для построения графиков обучения.

## Использование

Чтобы использовать этот код и провести эксперименты с различными функциями активации, выполните следующие шаги:

1. **Установка зависимостей:**
    Убедитесь, что у вас установлены необходимые библиотеки. Вы можете установить их с помощью следующей команды:

    ```bash
    pip install matplotlib tensorflow
    ```

2. **Запуск основного скрипта:**
    Запустите основной скрипт `main.py`, который содержит определения моделей, процесс обучения и оценку результатов. Используйте следующую команду:

    ```bash
    python main.py
    ```

3. **Анализ результатов:**
    После завершения обучения вы увидите графики потерь и точности для каждой модели. Эти графики могут помочь вам сравнить производительность моделей с разными функциями активации.

4. **Изменение параметров (по желанию):**
    Если вы хотите изменить параметры обучения или архитектуру моделей, вы можете отредактировать файл `main.py` в соответствии с вашими предпочтениями.

Обратите внимание, что результаты могут варьироваться в зависимости от конфигурации моделей и параметров обучения. Рекомендуется провести несколько экспериментов с различными настройками для получения наилучших результатов.

## Пример для 1 моделии 
#Обучение
![image](https://github.com/pmi31Roberto/Andrey_Anatolyevich/assets/120023351/0b5c40df-f5b6-4b7d-a1e1-804c2a166293)
#Графики
![image](https://github.com/pmi31Roberto/Andrey_Anatolyevich/assets/120023351/9e5ff93c-1735-45c0-b50a-daa5c01bc3aa)
