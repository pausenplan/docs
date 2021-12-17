# docs.pausenplan.de

Moduły:

+ account
+ account_list
+ user
+ user_list
+ token
+ token_list
+ time
+ time_list


## account

## resource
db::account

### Model:
+ Imię
+ Nazwisko
+ Rola []
+ Stanowisko
+ username 

### Funkcje:
+ signin()
+ signout()
+ update()


## account_signin

### View:
1. Formularz rejestracji konta użytkownika

## resource
db::account

### Funkcje:
+ signin()


## account_update

### View:
1. Zmiana danych konta

## resource
db::account

### Funkcje:
+ signout()



## account_signout

### View:
1. Usunięcie/zawieszenie konta/usunięcie danych po x dniach

## resource
db::account



## account_list

### View
1. Tabela z kontami, możliwość usunięcia/przywrócenia/blokady konta
2. Dane każdego konta

### Model:
+ AccountCollection

### Funkcje:
+ suspend()
+ delete()



## user

### View:
1. Formularz logowania
2. 

### Model:pausenplan
+ username
+ password
+ lista uprawnien aplikacji

### Funkcje:
+ login
+ loginout



## user_list

### View:
1. lista aktywnych użytkowników

### Model:
+ username
+ password

### Funkcje:
+ login
+ loginout


## user_setting



## user_rights




## user_token_list

### View:
1. lista zalogowanych użytkowników

### Model:
+ username
+ password

### Funkcje:
+ login
+ loginout

