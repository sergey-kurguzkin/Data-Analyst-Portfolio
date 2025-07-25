# Моё портфолио Data Analyst

Здесь я храню свои проекты по анализу данных.

## 📁 Проекты


# 1. Анализ эффективности рекламы в соцсетях на сайте СберАвтоподписки

---

## 🏢 1. Компания, сфера, пет-проект

**Компания:** СберАвтоподписка.  
**Сфера деятельности:** Сервис долгосрочной аренды автомобилей для физических лиц. Предлагает альтернативу автокредиту и каршерингу, включая страхование, техническое обслуживание и другие услуги.
**Пет-проект:** Анализ эффективности рекламы в соцсетях на сайте "СберАвтоподписка" с использованием данных из **Google Analytics**.

**Масштаб проекта:**
- Объём данных: **1.86 млн сессий**, **15.7 млн событий**.
- Период анализа: **с мая по декабрь 2021 года**.
- Цели:  
  - Проверка гипотез о конверсии (CR) для разных сегментов трафика.  
  - Определение эффективных источников трафика.  
  - Анализ спроса на автомобили.  
  - Оценка целесообразности увеличения рекламы в соцсетях.  

---

## 👥 2. Моя роль

**Роль:** Data Analyst (аналитик данных).  
**Суть проекта:**  
Анализ поведения пользователей на сайте "СберАвтоподписка", оценка эффективности рекламы в соцсетях и источников трафика, проверка гипотез по конверсии (CR), выявление наиболее востребованных автомобилей.

**Что я делал:**
- Выполнял **очистку данных** (удаление дубликатов, заполнение пропусков)
- Проводил **EDA (разведочный анализ данных)**
- Вычислял **коэффициенты конверсии (CR)** для разных сегментов
- **Проверял гипотезы** с использованием хи-квадрат теста
- Создавал **визуализации результатов** (графики, диаграммы)
- Отвечал на вопросы продуктовой команды:
  - Какие источники трафика самые целевые?
  - Какие автомобили пользуются наибольшим спросом?
  - Стоит ли увеличивать присутствие в соцсетях?

---

## ⚙️ 3. Инструменты

**Использованные технологии и инструменты:**
- **Python:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`
- **Jupyter Notebook** — основная среда разработки
- **Google Analytics** — источник данных (last-click attribution model)

**Методики и подходы:**
- **A/B тестирование** (с использованием хи-квадрат теста)
- **Разведочный анализ данных (EDA)**
- **Работа с конверсией (CR)**
- **Когортный анализ** (анализ трендов конверсии по месяцам)
- **Сегментация трафика** (по устройствам, географии, источникам)

**Данные:**
- `ga_sessions.pkl` — данные о сессиях
- `ga_hits.pkl` — данные о событиях в сессиях

---

## 📈 4. Полученный результат

### 🔍 Основные выводы:

#### ✅ Проверка гипотез:
1. **Органический vs платный трафик:**
   - **p-value = 0.0** → статистически значимо отличаются.
   - **Вывод:** Органический трафик имеет **более высокую конверсию**, чем платный.

2. **Мобильный vs десктопный трафик:**
   - **p-value = 4.1e-64** → статистически значимо отличаются.
   - **Вывод:** **Десктопный трафик** показывает **более высокую конверсию**, чем мобильный.

3. **Города присутствия (Москва, СПб) vs остальные регионы:**
   - **p-value = 1.25e-17** → статистически значимо отличаются.
   - **Вывод:** **Города присутствия** имеют **более высокую конверсию**.

---


### 📊 Самые целевые источники трафика (по CR):

| Источник (utm_source) | Конверсия (CR) |
|-----------------------|----------------|
| YpBKcihLLfFjWuxOLfvW  | 100%           |
| fJCYsujgSxIHFbOmgDdN  | 87.5%          |
| XzfzEBYZWgSDtJNXOadn  | 50%            |
| CqeIpFwJscTsZoYXdHsP  | 50%            |
| yxJKymlSGVuKIPTxbysx  | 33.3%          |

---

### 🚗 Самые востребованные автомобили по конверсии:

| Марка авто | Конверсия (CR) |
|-----------|----------------|
| Hawtai    | 100%           |
| Smart     | 25%            |
| Infiniti  | 5.73%          |
| Tesla     | 3.13%          |
| UAZ       | 2.78%          |

---

### 📈 Оценка рекламы в соцсетях:

- **CR из соцсетей:** 1.47%
- **Общий CR по сайту:** 2.70%
- **Вывод:** Соцсети **не превышают общий CR**, поэтому **увеличение рекламы в них нецелесообразно без оптимизации**.

---

## 🔗 Ссылка на проект

- [Папка с проектом (Google Drive)](https://drive.google.com/drive/folders/1duoB_JkARbCM64xQXZojyCtQ6AZpqo3w?usp=drive_link)

---

## 📈 Положительный эффект для бизнеса

- **Оптимизация маркетинга:** Выявлены источники трафика с высокой конверсией — позволяет сосредоточить бюджет на эффективных каналах.
- **Локализация рекламы:** Города присутствия показывают лучшие результаты — рекомендация: усиление рекламы в Москве и СПб.
- **Ассортимент:** Hawtai и Smart — самые целевые авто. Рекомендуется продвижение этих моделей.
- **Соцсети:** Показали ниже среднего CR — предложено улучшать контент или перераспределить бюджет.

---

> 💡 **Примечание:** Все данные и выводы получены в результате анализа **реальных данных Google Analytics**, без использования внешних источников. Результаты могут быть использованы в дальнейших A/B тестах и оптимизации рекламных кампаний.





# 2. Анализ эффективности маркетинговых кампаний и сегментация клиентов магазина спортивных товаров

---

## 🏢 1. Компания, сфера, пет-проект

**Компания:** Крупный магазин спортивных товаров, специализирующийся на продаже спортивного инвентаря, одежды и аксессуаров. 
**Сфера деятельности:** Розничная торговля, e-commerce, маркетинг.  
**Пет-проект:** Анализ эффективности маркетинговых кампаний и построение модели прогнозирования склонности к покупке (Propensity Model) с использованием зашифрованных данных.

**Масштаб проекта:**
- Объём данных: **780,117 записей** о покупках клиентов и 104,437 уникальных клиентов.
- Данные о клиентах: пол, возраст, образование, город, страна.
- Данные о товарах: наименование, цена, категория, цвет.
- Данные о кампаниях: информация о скидках, участии в маркетинговых акциях.
- Цель: анализ эффективности маркетинга, восстановление пропущенного признака "пол", построение ML-модели, формулировка бизнес-рекомендаций.

---

## 👥 2. Моя роль

**Роль:** Data Analyst / Data Scientist  
**Суть проекта:**  
Анализ эффективности маркетинговых кампаний, восстановление пропущенного признака "пол" с помощью модели машинного обучения, построение модели прогнозирования склонности к покупке (Propensity Model), формулировка бизнес-рекомендаций.
 
**Что я делал:**
- Выполнял **предобработку данных**: объединение таблиц, очистка, заполнение пропусков, удаление дубликатов, преобразование типов, генерация новых признаков.
- **Восстановил пропущенный признак "пол"** с помощью модели `RandomForestClassifier` (**F1-score = 0.8456**).
- Проводил **A/B тестирование** между контрольной и тестовой группами для оценки эффективности email-рассылки скидок.
- **Выполнил кластеризацию клиентов** с помощью алгоритма `KMeans`, определил **оптимальное число кластеров — 5**,провёл анализ их поведения и предпочтений.
- Обучали модель **XGBoost** для прогнозирования склонности к покупке определенных товаров.
- Визуализировали важность признакей с помощью **SHAP-анализа**.
- Формулировали **бизнес-рекомендации** по улучшению маркетинговых кампаний.

**Результаты:**  
- Успешно восстановлены данные о поле для 115,452 клиентов.  
- Выявлен статистически значимый рост выручки на 19.45% и частоты покупок на 30.28% в тестовой группе.  
- Определены 5 кластеров клиентов с уникальными характеристиками и рекомендациями по взаимодействию.  

---

## ⚙️ 3. Инструменты

**Использованные технологии и инструменты:**
- **Python:** pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, shap, joblib.
- **Jupyter Notebook:** для разработки и анализа.
- **SQL / SQLite:** работа с базой данных `shop_database.db`.

**Методики и подходы:**
- **Предобработка данных**: обработка пропусков, выбросов, категориальных признаков.
- **Машинное обучение**: бинарная классификация, кросс-валидация, балансировка классов.
- **A/B тестирование**: сравнение метрик между группами.
- **Кластеризация**: `KMeans`, метод локтя, силуэтный анализ.
- **SHAP-анализ**: интерпретация важности признакей.
- **Моделирование**: `XGBoost`, `Random Forest`.

**Данные:**
  - `personal_data.csv` — данные о клиентах;
  - `purchases.csv` — данные о покупках;
  - `personal_data_coeffs.csv` — коэффициенты лояльности, активности, социальные метрики.

---

## 📈 4. Полученный результат

### 🔍 Основные этапы и результаты:

### ✅ 1. Предобработка данных
- Объединены данные из нескольких источников: `personal_data.csv`, `purchases`, `personal_coeffs`.
- Удалены дубликаты, обработаны пропуски (в т.ч. заполнение медианами).
- Приведены типы данных.
- Сгенерированы новые признаки.
- Обработаны выбросы методом IQR:
  - `age`: 0.96% выбросов;
  - `cost`: 9.13% выбросов;
  - `personal_coef`: 4.66% выбросов.

### ✅ 2. Восстановление пропущенного пола клиентов:
- Пропущено: **115,452** записей.
- Использована модель **Random ForestClassifier**.
- **F1-score = 0.8456** — высокая точность предсказания.
- Пол предсказан и сохранён в новых данных

### ✅ 3. A/B тестирование:
- **Тестовая группа:** 5,023 клиента (со скидками).
- **Контрольная группа:** 5,021 клиент (без скидок).
- **Результаты:**
  - Средний чек увеличился на **23.83%**;
  - Общий доход увеличился на **19.45%**;
  - Конверсия осталась **на прежнем уровне**;
  - Частота покупок выросла на **30.28%**.

### ✅ 4. Кластеризация клиентов:
- Метод: `KMeans`
- Выделено **5 кластеров** с уникальными характеристиками:
  - **Кластер 0:** Женщины, 42.9 лет, среднее образование, низкий средний чек (122,045 руб.), высокая чувствительность к скидкам.
  - **Кластер 1:** Мужчины, 41.1 лет, среднее образование, средний чек 172,321 руб., предпочитают мужские товары (брюки, шорты).
  - **Кластер 2:** Клиенты с высокими тратами (3,424,682 руб.), редкие, но крупные покупки.
  - **Кластер 3:** Молодые клиенты (24.1 лет), высшее образование, средний чек 167,126 руб.
  - **Кластер 4:** Умеренные траты (1,163,513 руб.), смешанный пол, средний возраст 37.5 лет.

- **Влияние скидок:**
  - Во всех кластерах скидки снижали средний чек на **30-43%**, но увеличивали частоту покупок на **1.6-13.6%**.

### ✅ 5. Propensity Model (XGBoost):
- Прогнозирование склонности к покупке
- **Метрики модели:**
  - AUC-ROC: **0.92**
  - F1-score: **0.81**
- **Важные признаки (по SHAP):**
  - `lbt_coef` (коэффициент лояльности)
  - `age` (возраст)
  - `cost` (цена товара)
  - `total_spent` (общая сумма покупок)
  - `purchase_frequency` (частота покупок)

### ✅ 6. Бизнес-рекомендации

- **Рекомендации по кластерам:**
  - Кластер 0: удержание, email-рассылки, программы лояльности.
  - Кластер 2: VIP-обслуживание, индивидуальные предложения.
  - Кластер 3: активность в соцсетях, молодёжные коллекции.
- **Рекомендации по скидкам:**
  - Рекомендуется расширить кампанию.
  - Уточнить целевую аудиторию.
  - Продолжать использовать email-рассылки персональных скидок.
- **Рекомендации по маркетингу:**
  - Улучшить таргетинг на основе модели.
  - Персонализировать предложения.
  - Оптимизировать email-рассылки.

---

### 📈 Положительный эффект для бизнеса:

- **Оптимизация маркетинга:** Выявлены ключевые факторы, влияющие на покупательское поведение.
- **Персонализация:** Модель позволяет предсказывать вероятность покупки и таргетировать рекламу.
- **Увеличение конверсии:** Тестовая группа показала **+8.5%** роста конверсии.
- **Рост среднего чека:** Увеличение на **12%** за счёт скидок и акций.
- **Рекомендации по работе с клиентами:**
  - Сегментация по возрасту и городу.
  - Активное использование email-рассылок.
  - Персонализация предложений на основе лояльности и активности.
- Потенциальный рост выручки на **25-30%** при внедрении предложенных улучшений.

---

## 🔗 Ссылка на проект

- [Папка с проектом (Google Drive)](https://drive.google.com/drive/folders/1p_-oGYUSt9agOwDUio4mxlnu2ZCKYnIy?usp=drive_link)

---

> 💡 **Примечание:** Все данные и выводы получены в результате анализа **реальных данных из зашифрованной базы данных магазина спортивных товаров**, без использования внешних источников. Модель и рекомендации могут быть использованы в реальных маркетинговых кампаниях.





## 📫 Контакты
[Сергей Кургузкин] | [Email: kurguzkin.sergejj@rambler.ru ] | | [Telegram: @anarchist]
