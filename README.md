# GAS ML

Тестовое задание по машинному обучению: первичный анализ русскоязычных текстов и тематическое моделирование.

## Содержимое

- `ml_assignment.ipynb` — решение первой части: загрузка, проверка и очистка данных, EDA, TF-IDF + NMF, визуализация и выводы.
- `requirements.txt` — библиотеки проекта.

Источник данных: [MonoHime/ru_sentiment_dataset](https://huggingface.co/datasets/MonoHime/ru_sentiment_dataset).

## Запуск в Windows PowerShell

Откройте терминал в корне проекта:

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
New-Item -ItemType Directory -Force data/raw
```

Откройте `ml_assignment.ipynb` в VS Code с расширениями Python и Jupyter, выберите ядро `.venv` и выполните ячейки сверху вниз.

Ячейка загрузки читает CSV из Hugging Face и сохраняет копию в `data/raw/datasets.csv`. Для её запуска нужен доступ к интернету. Датасет и локальное окружение в репозиторий не включены.
