# Machine Learning Course (ML-4)

Репозиторій практичних та лабораторних робіт з курсу **Machine Learning**.

**Автор:** [Олександр Гріджак](https://github.com/OleksandrHridzhak)  

---

## 📌 Лабораторні роботи

- [x] **[Лабораторна робота 1: Лінійна регресія та оптимізація](lab1/)** — ✅ Виконано
  - Датасет: Ames Housing (*House Prices*)
  - Лінійна регресія з нуля на NumPy (Batch, SGD, Mini-batch GD)
  - Аналіз залишків ($R^2$, лінійність, нормальність, гомоскедастичність, VIF)

- [x] **[Лабораторна робота 2: Логістична регресія та федеративне навчання](lab2/)** — ✅ Виконано
  - Датасет: Dry Bean Dataset (UCI ID 602, 7 класів)
  - Багатокласова логістична регресія з нуля на NumPy (Softmax, Cross-Entropy Loss, Ridge)
  - Розподіл даних: IID та Non-IID (розподіл Діріхле $\alpha \in \{5.0, 1.0, 0.3\}$)
  - Федеративне навчання FedAvg: зважена агрегація та аналіз Client Drift

- [x] **[Лабораторна робота 3: Детекція згенерованого ШІ тексту (FastText + TF-IDF)](lab3/)** — ✅ Виконано
  - Датасет: AI vs Human Text Classification Dataset 2026 (Kaggle, 2000 текстів)
  - Попередня обробка тексту через SpaCy (`en_core_web_sm`, лематизація, видалення стоп-слів)
  - Навчання моделі субсловних ембеддінгів FastText (Gensim Skip-Gram)
  - Агрегація векторів: Mean Pooling vs TF-IDF Weighted Mean
  - Класифікація (SVM RBF, Logistic Regression, KNN) та геометричний аналіз t-SNE

---

## 📂 Структура репозиторію

```text
ml-4/
├── README.md                # Опис курсу та навігація
├── .gitignore
├── lab1/                    # Лабораторна 1 (Лінійна регресія)
│   ├── lab1.ipynb           # Ноутбук з кодом та висновками
│   ├── lab1.pdf             # PDF-звіт
│   ├── README.md            # Короткий звіт Lab 1
│   ├── ML-1-Practice.md     # Умова завдання
│   └── ...                  # Датасет
├── lab2/                    # Лабораторна 2 (Логістична регресія та FL)
│   ├── lab2.ipynb           # Ноутбук з моделлю, FedAvg та експериментами
│   ├── lab2.pdf             # PDF-звіт
│   ├── README.md            # Короткий звіт Lab 2
│   ├── ML-2-Practice.md     # Умова завдання
│   └── Dry_Bean_Dataset.csv # Датасет Dry Bean
└── lab3/                    # Лабораторна 3 (FastText, TF-IDF та детекція AI-тексту)
    ├── lab3.ipynb           # Ноутбук з експериментами, t-SNE та відповідями
    ├── lab3.pdf             # Згенерований PDF-звіт (24 стор.)
    ├── README.md            # Короткий звіт Lab 3
    ├── ML-3-Practice.md     # Умова завдання
    └── ai_vs_human_text_2026.csv # Датасет Kaggle
```

---

## 🚀 Встановлення та запуск

```bash
git clone https://github.com/OleksandrHridzhak/ml-4.git
cd ml-4
pip install numpy pandas matplotlib seaborn scipy scikit-learn spacy gensim jupyter
python -m spacy download en_core_web_sm

# Запуск Лабораторної роботи 3:
cd lab3
jupyter notebook lab3.ipynb
```
