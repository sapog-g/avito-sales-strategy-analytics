# Car Liquidity & Sales Strategy Optimization

## Project Overview
Это глубокое аналитическое исследование ликвидности подержанных автомобилей на платформе Avito. Цель проекта - выявить ключевые драйверы спроса и создать автоматизированный алгоритм для оптимизации платных услуг продвижения (VAS).

## Key Innovation: "Point of Decay" Algorithm
Главная ценность проекта - авторский алгоритм **Point of Decay**. Он математически вычисляет точку критической деградации органического спроса (падение интереса на 70% от пика). 
- Алгоритм позволяет не предлагать платные услуги слишком рано или безнадежным объявлениям.
- Определяет идеальное "окно" для VAS (обычно 4-6 день), максимизируя окупаемость продавца.

## Tech Stack & Methodology
- **Languages:** Python (Pandas, NumPy)
- **Visualization:** Plotly (interactive dashboards), Seaborn, Matplotlib.
- **ML Models:** Random Forest, LightGBM.
- **Advanced Analytics:** 
  - **SHAP & Feature Importance:** интерпретация нелинейных зависимостей.
  - **K-Means Clustering:** сегментация жизненного цикла объявлений.
  - **Bootstrapping:** проверка статистической значимости гипотез ($p < 0.001$).
  - **Sensitivity Analysis:** симуляция эластичности цены.

## Business Insights
1. **Price-to-Market (PTM):** Доказано, что выгода относительно рынка - доминирующий фактор ликвидности.
2. **Trust Factor:** Выявлено, что в Premium-сегменте рейтинг продавца ниже 4.0 полностью блокирует продажи.
3. **Mileage Anomaly:** Обнаружен сегмент "капсул времени" (авто 15+ лет с малым пробегом), имеющих аномально высокий спрос.

## Experiment Design
В проекте спроектирован **Geo-Split A/B тест** для валидации стратегии. Введена метрика **OEC (Overall Evaluation Criterion)**: *Incremental Contacts per VAS Ruble*.

---
### Author
**Сапоговский Георгий** 
- GitHub: @sapog-g
- Telegram: @sapog_g
