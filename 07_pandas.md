# 📌 Wprowadzenie do biblioteki Pandas

**Pandas** to potężna biblioteka w Pythonie służąca do analizy i manipulacji danymi. 
Umożliwia efektywne operacje na danych w formie tabelarycznej (DataFrame) oraz jednowymiarowych strukturach danych (Series).

## 🔹 Instalacja Pandas
```bash
pip install pandas

## 🔹 Importowanie Pandas
```python
import pandas as pd
```

## 🔹 Struktury danych w Pandas
### 🟢 Series – jednowymiarowa struktura danych
```bash
```python
# Tworzenie Series z listy
s = pd.Series([10, 20, 30, 40])
print(s)
```

### 🟢 DataFrame – dwuwymiarowa struktura danych
```bash
```python
# Tworzenie DataFrame ze słownika
data = {
    'Imię': ['Anna', 'Jan', 'Kasia'],
    'Wiek': [25, 30, 22],
    'Miasto': ['Warszawa', 'Kraków', 'Gdańsk']
}
df = pd.DataFrame(data)
print(df)
```


## 🔹 Wczytywanie i zapisywanie danych
```bash
```python
# Wczytywanie danych z pliku CSV
df = pd.read_csv('dane.csv')

# Zapisywanie DataFrame do pliku CSV
df.to_csv('wynik.csv', index=False)

# Wczytywanie danych z pliku Excel
df = pd.read_excel('dane.xlsx')
```


## 🔹 Podstawowe operacje na DataFrame
```bash
```python
# Wyświetlanie pierwszych i ostatnich wierszy
df.head()  # Pierwsze 5 wierszy
df.tail(3)  # Ostatnie 3 wiersze

# Informacje o danych
df.info()
df.describe()  # Statystyki opisowe

# Pobieranie kolumny
df['Imię']
```

## 🔹 Filtrowanie danych\
```bash
```python
# Filtrowanie wierszy
filtrowane = df[df['Wiek'] > 25]
print(filtrowane)
```


## 🔹 Grupowanie danych
```bash
```python
# Grupowanie po kolumnie 'Miasto'
grupa = df.groupby('Miasto').mean()
print(grupa)
```

## 🔹 Modyfikacja danych
```bash
```python
# Dodanie nowej kolumny
df['Pensja'] = [5000, 6000, 4500]

# Usunięcie kolumny
df.drop(columns=['Pensja'], inplace=True)
```

