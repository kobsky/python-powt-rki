# 📌 Instrukcje sterujące w Pythonie

## 🔹 Instrukcje warunkowe
```bash
```python
# Instrukcja if-elif-else 
x = 10
if x > 0:
    print("Liczba dodatnia")
elif x == 0:
    print("Zero")
else:
    print("Liczba ujemna")
```

## 🔹 Pętle
```bash
```python
# Pętla for - iteracja po elementach listy
lista = [1, 2, 3, 4]
for element in lista:
    print(element)

# Pętla for - iteracja po zakresie liczb
for i in range(5):
    print(i)  # Wypisze liczby od 0 do 4

# Pętla while
licznik = 0
while licznik < 3:
    print("Licznik:", licznik)
    licznik += 1
```


## 🔹 Instrukcje sterujące przepływem pętli
```bash
```python
# Przerywanie pętli - instrukcja break
for liczba in range(10):
    if liczba == 5:
        break  # Przerwie działanie pętli
    print(liczba)

# Pomijanie iteracji - instrukcja continue
for liczba in range(5):
    if liczba == 2:
        continue  # Pomiń iterację, ale nie kończ pętli
    print(liczba)
```

