# docs.pausenplan.de

Moduły:

+ account
+ account_list
+ account_update
+ account_signin
+ account_signout
+ user
+ user_list

+ token
+ token_list
+ time
+ time_list



## account

Atrybuty:
+ Imię
+ Nazwisko
+ Rola []
+ Stanowisko
+ username

Funkcje:
set*
get*

zamiast account entity
zastosowac kolekcje pojedynczych parametrow

+ FirstName
+ LastName
+ TeamRole
+ WorkPosition
+ UserName

```php
class Controller{

  // Collection
  AccountCollection = new Collection(FirstName, LastName, TeamRole, WorkPosition, UserName)
  
  // Resource
  DbResource = new Db()

  // Query Command
  function AccountCreate() {
    return new Event(
      new Create(AccountCollection, DbResource)
    )
  )

}
```

## account_db

## resource/connector
db::account

## entities:
account

### Funkcje:
+ create()
+ read()
+ update()
+ delete()



## account_create

### View:
1. Zmiana danych konta

## resource
db::account

### Funkcje:
+ signin(account)


## account_update

### View:
1. Zmiana danych konta

## resource
db::account

### Funkcje:
+ signout()





## account_signin

### View:
1. Formularz rejestracji konta użytkownika

## resource
db::account

### Funkcje:
+ signin()



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

