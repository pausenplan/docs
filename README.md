# docs.pausenplan.de

## moduły:
+ account
+ user
+ token
+ time


## account

### View:
Formularz rejestracji konta użytkownika

### Model:
+ Imię
+ Nazwisko
+ Rola []

+ Stanowisko 

### Funkcje:
+ signin()
+ signout()


## accounts

### View
Tabela z kontami, możliwość usunięcia/przywrócenia/blokady konta

### Model:
+ AccountCollection

### Funkcje:
+ suspend()
+ delete()



## user

### View:
Formularz logowania

### Model:
+ username
+ password

### Funkcje:
+ login
+ loginout


