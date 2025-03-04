# 📌 Funkcje w Pythonie

## 🔹 Definiowanie funkcji
```bash
```python
# Definiowanie prostej funkcji
def przywitaj():
    print("Cześć! Witaj w Pythonie.")

# Wywołanie funkcji
przywitaj()
```

## 🔹 Funkcja z argumentami
```bash
```python
# Funkcja przyjmująca argumenty
def dodaj(a, b):
    return a + b

wynik = dodaj(5, 3)
print("Wynik dodawania:", wynik)
```

## 🔹 Argumenty domyślne
```bash
```python
# Funkcja z argumentem domyślnym
def przedstaw_sie(imie="Anonim"):
    print("Cześć, mam na imię", imie)

przedstaw_sie("Jan")  # Cześć, mam na imię Jan
przedstaw_sie()  # Cześć, mam na imię Anonim
```


## 🔹 Argumenty pozycyjne i nazwane
```bash
```python
# Argumenty pozycyjne
print("Python", "jest", "super!")  # Python jest super!

# Argumenty nazwane
def powitanie(imie, wiek):
    print(f"Cześć {imie}, masz {wiek} lat.")

powitanie(imie="Anna", wiek=25)
```


## 🔹 Funkcje zwracające wiele wartości
```bash
```python
# Funkcja zwracająca wiele wartości
def operacje(a, b):
    suma = a + b
    roznica = a - b
    return suma, roznica

wynik1, wynik2 = operacje(10, 4)
print("Suma:", wynik1, "Różnica:", wynik2)
```
