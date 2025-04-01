# Hello World Web

## Opis projektu
Hello World Web to prosty projekt webowy, który wyświetla stronę z napisem "Hello, World!". Jest to podstawowy przykład aplikacji webowej, który można uruchomić lokalnie za pomocą Python Flask.

## Wymagania
Przed rozpoczęciem instalacji upewnij się, że masz zainstalowane:
- Python 3.8 lub nowszy
- pip (menedżer pakietów Pythona)

## Instalacja
1. Sklonuj repozytorium:
   ```sh
   git clone https://github.com/username/hello-world-web.git
   cd hello-world-web
   ```

2. Utwórz i aktywuj wirtualne środowisko:
   ```sh
   python -m venv venv
   source venv/bin/activate  # dla systemu Linux/MacOS
   venv\Scripts\activate     # dla systemu Windows
   ```

3. Zainstaluj wymagane pakiety:
   ```sh
   pip install -r requirements.txt
   ```

## Uruchomienie aplikacji
1. W terminalu uruchom serwer:
   ```sh
   python app.py
   ```
2. Otwórz przeglądarkę i przejdź do adresu:
   ```
   http://127.0.0.1:5000
   ```
3. Powinna się wyświetlić strona z napisem "Hello, World!".

## Struktura projektu
```
hello-world-web/
│── app.py
│── requirements.txt
│── templates/
└── README.md
```

## Skrypt aplikacji (app.py)
```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "Hello, World!"

if __name__ == '__main__':
    app.run(debug=True)
```

## Autor
Dariusz Kisiel

## Licencja
Ten projekt jest udostępniany na licencji MIT.

