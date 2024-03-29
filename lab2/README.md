# Лабораторная работа 2: Построение моделей на основе предобученных эмбеддингов

## Цель работы
Научиться работать с предобученными моделями и на основе предобученных эмбеддингов строить новые модели.

## 1. Подготовка данных

### 1.1 Загрузка датасета
Для выполнения работы был использован датасет из YouTube, содержащий аудиозаписи в четырех категориях: 'travel', 'food', 'art_music', 'history'. Каждая категория содержала от 25 до 30 треков продолжительностью по 10-20 минут.

### 1.2 Фильтрация и обработка данных
Аудиозаписи были разбиты на небольшие сегменты длиной по 5 секунд, и для каждого сегмента были получены эмбеддинги.

## 2. Разработка модели
На основе полученных эмбеддингов была обучена нейронная сеть Wav2Vec2. Модель была обучена для классификации аудиосегментов по категориям 'travel' и 'not travel'.

## 3. Оценка качества модели
### 3.1 Метрики
Модель была оценена на тестовом наборе данных с использованием метрик точности (Accuracy) и F1-меры.

### 3.2 Результаты
После 100 эпох обучения были получены следующие результаты:
```plaintext
Accuracy: 82.33%
F1-мера: 0.35
```

## 4. Выводы по работе
Лабораторная работа была посвящена построению моделей на основе предобученных эмбеддингов. Для этого использовался датасет с аудиозаписями из YouTube, разделенный на категории 'travel', 'food', 'art_music' и 'history'. Аудиозаписи были обработаны, разбиты на сегменты, и для каждого получены эмбеддинги.
На основе этих эмбеддингов была обучена модель Wav2Vec2, успешно классифицировавшая аудиосегменты.


---

**Исходный код:** [Lab2.ipynb](Lab2.ipynb)

**Автор:** Батурина Ксения, M4130

**Лицензия:** Этот проект распространяется под MIT License
