
# 📌 Programowanie obiektowe w Pythonie

Programowanie obiektowe (OOP) to paradygmat, który pozwala na organizację kodu w klasy i obiekty. 
Python w pełni wspiera OOP, umożliwiając tworzenie elastycznych i czytelnych programów.

## 🔹 Definiowanie klasy i tworzenie obiektów
```bash
```python
# Definicja klasy
class Samochod:
    def __init__(self, marka, model, rok):
        self.marka = marka
        self.model = model
        self.rok = rok

    def opis(self):
        return f"Samochód: {self.marka} {self.model} ({self.rok})"

# Tworzenie obiektu
auto = Samochod("Toyota", "Corolla", 2020)
print(auto.opis())

## 🔹 Modyfikowanie atrybutów obiektu
```python
# Zmiana wartości atrybutu
auto.rok = 2022
print(auto.opis())


## 🔹 Dziedziczenie – tworzenie klas pochodnych
```bash
```python
class ElektrycznySamochod(Samochod):
    def __init__(self, marka, model, rok, bateria):
        super().__init__(marka, model, rok)
        self.bateria = bateria

    def opis_baterii(self):
        return f"Pojemność baterii: {self.bateria} kWh"

# Tworzenie obiektu klasy pochodnej
e_auto = ElektrycznySamochod("Tesla", "Model S", 2022, 100)
print(e_auto.opis())
print(e_auto.opis_baterii())
```bash

## 🔹 Metody statyczne i klasy
```bash
```python
class Kalkulator:
    @staticmethod
    def dodaj(a, b):
        return a + b

print(Kalkulator.dodaj(5, 3))
```


