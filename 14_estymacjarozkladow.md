# 📌 Estymacja parametrów rozkładów w Pythonie

Estymacja parametrów rozkładów statystycznych to proces dopasowania modelu probabilistycznego do danych. 
W Pythonie można to zrobić przy użyciu **NumPy** i **SciPy**.

## 🔹 Generowanie danych do analizy
```bash
```python
import numpy as np
import matplotlib.pyplot as plt
import scipy.stats as stats

# Generowanie danych z rozkładu normalnego
data = np.random.normal(loc=50, scale=10, size=1000)

# Wizualizacja histogramu
plt.hist(data, bins=30, density=True, alpha=0.6, color='g')
plt.title("Histogram danych")
plt.xlabel("Wartości")
plt.ylabel("Częstotliwość")
plt.show()
```

## 🔹 Dopasowanie rozkładu normalnego do danych
```bash
```python
# Estymacja średniej i odchylenia standardowego
mean, std = np.mean(data), np.std(data)
print(f"Średnia: {mean}, Odchylenie standardowe: {std}")
```

## 🔹 Dopasowanie rozkładu normalnego przy użyciu `scipy.stats`
```bash
```python
# Dopasowanie rozkładu normalnego
dist = stats.norm.fit(data)  # Zwraca (średnia, odchylenie standardowe)
print(f"Parametry dopasowanego rozkładu: Średnia={dist[0]}, Odchylenie standardowe={dist[1]}")
```


## 🔹 Wykres dopasowanego rozkładu
```bash
```python
xmin, xmax = min(data), max(data)
x = np.linspace(xmin, xmax, 100)
pdf = stats.norm.pdf(x, *dist)

plt.hist(data, bins=30, density=True, alpha=0.6, color='g')
plt.plot(x, pdf, 'k', linewidth=2)
plt.title("Dopasowany rozkład normalny")
plt.xlabel("Wartości")
plt.ylabel("Prawdopodobieństwo")
plt.show()
```


## 🔹 Dopasowanie innych rozkładów (np. wykładniczy, gamma)
```bash
```python
# Dopasowanie rozkładu wykładniczego
dist_exp = stats.expon.fit(data)
print(f"Parametry rozkładu wykładniczego: {dist_exp}")

# Dopasowanie rozkładu gamma
dist_gamma = stats.gamma.fit(data)
print(f"Parametry rozkładu gamma: {dist_gamma}")
```

