# Instalacja django na Windows

### 0. Instalacja Pythona
---------------------------
a)
Wejdź na stronę: https://www.python.org/downloads/

b)
Pobierz i zainstaluj Pythona

c)
Otwórz wiersz polecenia i wpisz:
>python
Powinno ukazać się to:
```
C:\Users\Janusz>python
Python 2.7.13 (v2.7.13:a06454b1afa1, Dec 17 2016, 20:42:59) [MSC v.1500 32 bit (Intel)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
### 1. Instalacja Virtualenv (Wirtualne środowisko)
-------------------------------------
a)
Wejdź na stronę: https://pypi.python.org/pypi/virtualenv

b)
Pobierz: virtualenv-15.1.0.tar.gz (md5, pgp)

c)
Wypakuj pobrane archiwum: virtualenv-15.1.0.tar.gz

d)
Otwórz wiersz poleceń i przejdź do katalogu w którym masz rozpakowane archiwum:
```
C:\Users\Janusz>cd C:\Users\Janusz\Downloads\dist\virtualenv-15.1.0
```
e)
Zainstaluj Virtualenv
```
C:\Users\Janusz\Downloads\dist\virtualenv-15.1.0>python setup.py install
```
### 2. Utwórz i aktywuj wirtualne środowisko
-----------------------------------------------------------------------------
a)
Utwórz wirtyalne środowisko nazywając je: "myenv"
```
C:\Users\Janusz>python -m virtualenv myenv
C:\Users\Janusz>dir
```
b)
Aktywuj wirtualne środowisko "myenv"
```
C:\Users\Janusz>.\myenv\Scripts\activate
(myenv) C:\Users\Janusz
```
### 3. Instalacja django
-----------------------------
a)
Zainstaluj django
```
(myenv) C:\Users\Janusz>pip install django
Collecting django
  Downloading Django-1.8.5-py2.py3-none-any.whl (6.2MB)
    100% |################################| 6.2MB 48kB/s
Installing collected packages: django
Successfully installed django-1.11.1
(myenv) C:\Users\Janusz>
```
b)
Otwórz wiersz polecenia i wpisz:
```
(myenv) C:\Users\Janusz>python
Python 2.7.13 (v2.7.13:a06454b1afa1, Dec 17 2016, 20:42:59) [MSC v.1500 32 bit (Intel)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> import django
>>> print(django.get_version())
1.11.1
```
>>>
