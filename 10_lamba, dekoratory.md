# 📌 Funkcje lambda, dekoratory i list comprehensions

## 🔹 Funkcje lambda – anonimowe funkcje
Funkcja `lambda` to krótka, jednowierszowa funkcja anonimowa.
```bash
```python
# Przykładowa funkcja lambda
suma = lambda x, y: x + y
print(suma(5, 3))  # 8

# Lambda jako argument funkcji
numbers = [1, 2, 3, 4, 5]
kwadraty = list(map(lambda x: x ** 2, numbers))
print(kwadraty)  # [1, 4, 9, 16, 25]
```

## 🔹 List comprehensions – skrócony zapis pętli
```bash
```python
# Tworzenie listy kwadratów liczb od 0 do 9
kwadraty = [x ** 2 for x in range(10)]
print(kwadraty)  # [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]

# List comprehension z warunkiem
parzyste = [x for x in range(10) if x % 2 == 0]
print(parzyste)  # [0, 2, 4, 6, 8]
```

## 🔹 Dekoratory – funkcje modyfikujące inne funkcje
```bash
```python
# Definiowanie dekoratora
def dekorator(func):
    def wrapper():
        print("Przed wywołaniem funkcji")
        func()
        print("Po wywołaniu funkcji")
    return wrapper

@dekorator
def przyklad():
    print("To jest funkcja docelowa")

przyklad()
```

## 🔹 Dekorator przyjmujący argumenty
```bash
```python
def powiel_tekst(n):
    def dekorator(func):
        def wrapper():
            print(func() * n)
        return wrapper
    return dekorator

@powiel_tekst(3)
def powitanie():
    return "Cześć! "

powitanie()
```



