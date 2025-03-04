# 📌 Wprowadzenie do biblioteki NumPy

**NumPy** (Numerical Python) to biblioteka do obliczeń numerycznych w Pythonie. 
Umożliwia operacje na wielowymiarowych tablicach i macierzach oraz oferuje funkcje matematyczne do ich efektywnej manipulacji.

## 🔹 Instalacja NumPy
```bash
pip install numpy

## 🔹 Importowanie NumPy
```python
import numpy as np
```

## 🔹 Tworzenie tablic NumPy
```bash
```python
# Tworzenie tablicy jednowymiarowej (wektora)
arr1 = np.array([1, 2, 3, 4, 5])
print(arr1)

# Tworzenie tablicy dwuwymiarowej (macierzy)
arr2 = np.array([[1, 2, 3], [4, 5, 6]])
print(arr2)

# Tworzenie tablicy wypełnionej zerami
zeros = np.zeros((3, 3))
print(zeros)

# Tworzenie tablicy wypełnionej jedynkami
ones = np.ones((2, 4))
print(ones)

# Tworzenie tablicy wypełnionej losowymi liczbami
rand_arr = np.random.rand(3, 3)
print(rand_arr)
```

## 🔹 Właściwości tablic NumPy
```bash
```python
arr = np.array([[1, 2, 3], [4, 5, 6]])
print("Kształt tablicy:", arr.shape)  # (2, 3) - 2 wiersze, 3 kolumny
print("Liczba wymiarów:", arr.ndim)  # 2
print("Typ danych:", arr.dtype)  # np.int32 lub np.int64
print("Liczba elementów:", arr.size)  # 6
```


## 🔹 Indeksowanie i wycinanie (slicing)
```bash
```python
arr = np.array([10, 20, 30, 40, 50])
print(arr[0])  # Pierwszy element
print(arr[-1])  # Ostatni element
print(arr[1:4])  # Elementy od indeksu 1 do 3
```


## 🔹 Operacje na tablicach NumPy
```bash
```python
# Dodawanie, odejmowanie, mnożenie i dzielenie tablic
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])
print(arr1 + arr2)  # [5 7 9]
print(arr1 - arr2)  # [-3 -3 -3]
print(arr1 * arr2)  # [4 10 18]
print(arr1 / arr2)  # [0.25 0.4 0.5]
```


## 🔹 Operacje na macierzach
```bash
```python
# Transpozycja macierzy
arr = np.array([[1, 2, 3], [4, 5, 6]])
print(arr.T)

# Iloczyn skalarny macierzy
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])
print(np.dot(A, B))
```

## 🔹 Statystyka i operacje matematyczne
```bash
```python
arr = np.array([1, 2, 3, 4, 5])
print(np.mean(arr))  # Średnia
print(np.median(arr))  # Mediana
print(np.std(arr))  # Odchylenie standardowe
print(np.sum(arr))  # Suma wartości
print(np.min(arr))  # Minimalna wartość
print(np.max(arr))  # Maksymalna wartość
```






