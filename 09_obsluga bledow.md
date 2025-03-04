# 📌 Obsługa błędów w Pythonie

**Obsługa błędów** pozwala na przechwytywanie i reagowanie na nieoczekiwane sytuacje w programie, zapobiegając jego awarii. 
Python oferuje mechanizmy do obsługi wyjątków poprzez `try-except`.

## 🔹 Podstawowa obsługa wyjątków
```python
try:
    x = 10 / 0  # Próba dzielenia przez zero
except ZeroDivisionError:
    print("Nie można dzielić przez zero!")


## 🔹 Obsługa wielu wyjątków
```bash
```python
try:
    liczba = int("abc")  # Konwersja błędnego stringa na int
except ValueError:
    print("Błąd konwersji: podana wartość nie jest liczbą.")
except ZeroDivisionError:
    print("Nie można dzielić przez zero.")
```
## 🔹 Użycie bloku `else` i `finally`
```bash
```python
try:
    plik = open("plik.txt", "r")
    zawartosc = plik.read()
    print(zawartosc)
except FileNotFoundError:
    print("Plik nie istnieje.")
else:
    print("Operacja zakończona sukcesem.")
finally:
    print("To wykonuje się zawsze, niezależnie od błędu.")
```

## 🔹 Podnoszenie wyjątków (`raise`)
```bash
```python
def sprawdz_wiek(wiek):
    if wiek < 18:
        raise ValueError("Musisz mieć co najmniej 18 lat.")
    return "Dostęp przyznany."

try:
    print(sprawdz_wiek(16))
except ValueError as e:
    print("Błąd:", e)
```



