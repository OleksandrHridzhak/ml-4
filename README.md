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
└── lab2/                    # Лабораторна 2 (Логістична регресія та FL)
    ├── lab2.ipynb           # Ноутбук з моделлю, FedAvg та експериментами
    ├── lab2.pdf             # PDF-звіт
    ├── README.md            # Короткий звіт Lab 2
    ├── ML-2-Practice.md     # Умова завдання
    └── Dry_Bean_Dataset.csv # Датасет Dry Bean
```

---

## 🚀 Встановлення та запуск

```bash
git clone https://github.com/OleksandrHridzhak/ml-4.git
cd ml-4
pip install numpy pandas matplotlib seaborn scipy scikit-learn jupyter

# Запуск Лабораторної роботи 2:
cd lab2
jupyter notebook lab2.ipynb
```
