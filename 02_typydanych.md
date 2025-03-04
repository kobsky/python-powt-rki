## 📌 Typy danych w Pythonie

### 🔹 Podstawowe typy danych
```python
# Liczby całkowite (int)
liczba_calkowita = 42

# Liczby zmiennoprzecinkowe (float)
liczba_zmiennoprzecinkowa = 3.14

# Łańcuchy znaków (str)
tekst = "Witaj w Pythonie!"

# Wartości logiczne (bool)
prawda = True
falsz = False

### 🔹 Typy sekwencyjne
```python
# Listy - dynamiczne tablice
lista = [1, 2, 3, 4, "tekst"]

# Krotki - niezmienne sekwencje
krotka = (10, 20, 30)

# Słowniki - klucz: wartość
slownik = {"imie": "Jan", "wiek": 25}

# Zbiory - unikalne wartości
zbior = {1, 2, 3, 3, 4}  # Wynik: {1, 2, 3, 4}


### 🔹 Konwersja typów
```python
# Zamiana liczby na string
liczba = 123
tekst = str(liczba)

# Zamiana stringa na liczbę
liczba_int = int("42")
liczba_float = float("3.14")


### 🔹 Operacje na ciągach znaków
```python
tekst = "Python jest super!"
print(tekst.upper())  # WIELKIE LITERY
print(tekst.lower())  # małe litery
print(tekst.replace("super", "świetny"))  # Zamiana słów
print(len(tekst))  # Długość tekstu


### 🔹 Sprawdzanie typu zmiennej
```python
print(type(liczba_calkowita))  # <class 'int'>
print(type(tekst))  # <class 'str'>
print(type(lista))  # <class 'list'>

