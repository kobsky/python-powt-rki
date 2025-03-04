# 📌 Wizualizacja danych w Pythonie

Biblioteki takie jak **Matplotlib** i **Seaborn** pozwalają na tworzenie wykresów i wizualizacji danych. 
Są one kluczowe do analizy danych i prezentowania wyników.

## 🔹 Instalacja Matplotlib i Seaborn
```bash
pip install matplotlib seaborn


## 🔹 Importowanie bibliotek
```python
import matplotlib.pyplot as plt
import seaborn as sns


## 🔹 Tworzenie prostego wykresu liniowego
```bash
```python
x = [1, 2, 3, 4, 5]
y = [10, 20, 25, 30, 40]

plt.plot(x, y, marker='o', linestyle='-', color='b', label='Dane')
plt.xlabel("X")
plt.ylabel("Y")
plt.title("Wykres liniowy")
plt.legend()
plt.show()
```


## 🔹 Wykres słupkowy
```bash
```python
kategorie = ['A', 'B', 'C', 'D']
wartosci = [10, 15, 7, 12]

plt.bar(kategorie, wartosci, color='green')
plt.xlabel("Kategorie")
plt.ylabel("Wartości")
plt.title("Wykres słupkowy")
plt.show()
```


## 🔹 Wykres kołowy
```bash
```python
udzialy = [35, 25, 25, 15]
labels = ['A', 'B', 'C', 'D']

plt.pie(udzialy, labels=labels, autopct='%1.1f%%', colors=['red', 'blue', 'green', 'purple'])
plt.title("Wykres kołowy")
plt.show()
```

## 🔹 Wizualizacja danych z Seaborn
```bash
```python
import pandas as pd

# Tworzenie przykładowego DataFrame
data = {
    'Kategoria': ['A', 'B', 'A', 'B', 'A', 'B'],
    'Wartość': [10, 15, 12, 18, 8, 20]
}
df = pd.DataFrame(data)

sns.barplot(x='Kategoria', y='Wartość', data=df)
plt.title("Wykres słupkowy Seaborn")
plt.show()
```

## 🔹 Histogram – rozkład danych
```bash
```python
import numpy as np

dane = np.random.randn(1000)
plt.hist(dane, bins=30, color='blue', edgecolor='black')
plt.title("Histogram rozkładu danych")
plt.xlabel("Wartości")
plt.ylabel("Częstotliwość")
plt.show()
```

