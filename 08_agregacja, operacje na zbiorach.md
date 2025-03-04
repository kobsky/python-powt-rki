# 📌 Agregacja danych w Pandas

**Agregacja danych** pozwala na podsumowywanie i analizę dużych zbiorów danych. Pandas oferuje wiele metod do grupowania i obliczania statystyk na danych.

## 🔹 Wczytywanie przykładowych danych
```bash
```python
import pandas as pd

# Tworzenie przykładowego DataFrame
data = {
    'Imię': ['Anna', 'Jan', 'Kasia', 'Piotr', 'Marek'],
    'Wiek': [25, 30, 22, 40, 35],
    'Miasto': ['Warszawa', 'Kraków', 'Gdańsk', 'Warszawa', 'Kraków'],
    'Pensja': [5000, 6000, 4500, 7000, 5500]
}
df = pd.DataFrame(data)
print(df)
```

## 🔹 Podstawowe operacje agregacyjne
```bash
```python
# Obliczanie średniej wartości dla kolumny 'Pensja'
print(df['Pensja'].mean())

# Obliczanie sumy wartości w kolumnie 'Pensja'
print(df['Pensja'].sum())

# Maksymalna i minimalna wartość
print(df['Pensja'].max())
print(df['Pensja'].min())
```


## 🔹 Grupowanie danych (`groupby`)
```bash
```python
# Średnia pensja w każdym mieście
grupowane = df.groupby('Miasto')['Pensja'].mean()
print(grupowane)

# Zliczanie ilości wystąpień w każdej grupie
print(df.groupby('Miasto').size())
```


## 🔹 Filtrowanie po grupach
```bash
```python
# Pobieranie tylko grupy Warszawa
grupa_warszawa = df[df['Miasto'] == 'Warszawa']
print(grupa_warszawa)
```


