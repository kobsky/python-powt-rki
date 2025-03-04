# 📌 Statystyka i generowanie liczb losowych w Pythonie

Python oferuje wbudowane moduły do obliczeń statystycznych oraz generowania liczb losowych. 
Najczęściej używane to **random** (dla liczb losowych) oraz **numpy** i **scipy.stats** (dla zaawansowanej statystyki).

## 🔹 Generowanie liczb losowych – moduł `random`
```bash
```python
import random

# Losowa liczba całkowita z zakresu (min, max)
print(random.randint(1, 100))

# Losowa liczba zmiennoprzecinkowa z zakresu (0, 1)
print(random.random())

# Losowa liczba zmiennoprzecinkowa z określonego zakresu
print(random.uniform(1, 10))

# Losowy wybór z listy
kolory = ['czerwony', 'zielony', 'niebieski']
print(random.choice(kolory))
```


## 🔹 Tworzenie losowych list
```bash
```python
# Losowa próbka elementów z listy
liczby = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(random.sample(liczby, 3))

# Tasowanie listy
random.shuffle(liczby)
print(liczby)
```


## 🔹 Statystyka w NumPy
```bash
```python
import numpy as np

# Tworzenie przykładowej tablicy danych
data = np.array([10, 20, 30, 40, 50, 60])

# Średnia, mediana, odchylenie standardowe
print(np.mean(data))  # Średnia
print(np.median(data))  # Mediana
print(np.std(data))  # Odchylenie standardowe
```


## 🔹 Rozkłady prawdopodobieństwa – `scipy.stats`
```bash
```python
from scipy.stats import norm

# Generowanie danych z rozkładu normalnego
dane = norm.rvs(loc=0, scale=1, size=1000)

# Obliczanie wartości prawdopodobieństwa dla danego punktu
print(norm.pdf(0))  # Gęstość prawdopodobieństwa w punkcie 0

# Dystrybuanta rozkładu normalnego
print(norm.cdf(0))  # Prawdopodobieństwo uzyskania wartości <= 0
```

