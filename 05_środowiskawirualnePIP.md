# 📌 Zarządzanie środowiskami wirtualnymi i pakietami w Pythonie

## 🔹 Tworzenie i zarządzanie środowiskiem wirtualnym
```bash
# Sprawdzenie wersji Pythona
python --version

# Instalacja modułu virtualenv (jeśli nie jest zainstalowany)
pip install virtualenv

# Tworzenie środowiska wirtualnego
python -m venv my_env

# Aktywowanie środowiska (Windows)
my_env\Scripts\activate

# Aktywowanie środowiska (Linux/macOS)
source my_env/bin/activate

# Dezaktywowanie środowiska wirtualnego
deactivate
```

## 🔹 Zarządzanie pakietami z pip
```bash
# Instalacja pakietu
pip install nazwa_pakietu

# Instalacja konkretnej wersji pakietu
pip install nazwa_pakietu==1.2.3

# Lista zainstalowanych pakietów
pip list

# Zapisywanie zainstalowanych pakietów do pliku
pip freeze > requirements.txt

# Instalacja pakietów z pliku requirements.txt
pip install -r requirements.txt

# Odinstalowanie pakietu
pip uninstall nazwa_pakietu
```

## 🔹 Sprawdzanie lokalizacji pakietów
```bash
# Sprawdzenie, gdzie Python szuka pakietów
python -m site --user-site

# Sprawdzenie ścieżki do konkretnego pakietu
python -c "import numpy; print(numpy.__file__)"
```

