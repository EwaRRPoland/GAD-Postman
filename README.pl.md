# GAD - Wdrażanie lokalne:

## Wymagania:

- Zainstalowany `Node.js` w systemie,

- Przetestowane na `Node.js` w wersjach 18 i 20,

- Zainstalowany `Git` w systemie.

## Pierwsze użycie:

1. Otwórz katalog główny projektu w wierszu poleceń lub terminalu.

2. Sklonuj repozytorium za pomocą komendy `git clone <adres repozytorium>` Jest to preferowany sposób korzystania z tej aplikacji.

3. Uruchom `npm i`, aby zainstalować moduły (nie używaj globalnych pakietów Node.js!).

4. Uruchom `npm run start`, aby uruchomić aplikację `GAD`.
5. Aplikacja będzie dostępna pod adresem `http://localhost:3000`.

## Aktualizacja wersji:

1. Jeśli korzystasz z paczki ZIP:

- Pobierz spakowane repozytorium.
- Rozpakuj je i zastąp swoją lokalną instancję `GAD`.
- Uruchom `npm i` w katalogu głównym, aby zainstalować nowe moduły.
- Uruchom `npm run start`, aby ponownie uruchomić `GAD`.

2. Jeśli korzystasz z klonowanego repozytorium:

- Otwórz katalog główny projektu w wierszu poleceń lub terminalu.
- Wykonaj `git pull`, aby pobrać najnowsze zmiany.
- Uruchom `npm i`, aby zainstalować nowe moduły.
- Uruchom `npm run start`, aby ponownie uruchomić `GAD`.

3. Aktualizacja wersji w przypadku zmian (np. w bazie danych):

- Jedną z możliwości jest zresetowanie wszystkich lokalnych zmian i pobranie nowej wersji.
  Należy jednak pamiętać, że w ten sposób utracisz wszystkie lokalne zmiany i dane!
- Otwórz katalog główny projektu w wierszu poleceń lub terminalu.
- Wykonaj polecenia:

```
git reset --hard HEAD
git pull
```

- Uruchom `npm i`, aby zainstalować nowe moduły.
- Uruchom `npm run start`, aby ponownie uruchomić `GAD`.

Na podstawie [instrukcji do GAD](https://github.com/jaktestowac/gad-gui-api-demo/blob/main/README.md)

## Aby uruchomić Swagger GAD:

- Uruchom `npm run start`, aby uruchomić aplikację `GAD`,

- Aplikacja będzie dostępna pod adresem `http://localhost:3000`,

- Wejdz na adres `http://localhost:3000/tools/swagger.html` znajdziesz tam Swagger GAD.

# Testowanie w Postman"

## Aby dokonać uwierzytelnienia w Postman:

- przy uzupełnianiu `request` w `Authorization` wybieramy typ `Bearer Token` i wklejamy wygenerowany `access_token` z `request` do logowania.

## Należy zaplanować przejrzystą strukturę zapytań:

- w katalogach należy umieścić poszczególne sekcje i w nich odpowiadające metody protokołu HTTP oraz `Request URL` pobrany ze `Swagger GAD`:

![](https://github.com/EwaRRPoland/GAD-Postman/blob/9e9d0264ed60d6d854a2c5320104c23aa351c237/assets/GadPostman_requests.jpg)

- do `request` możemy dołaczy testy:

![](https://github.com/EwaRRPoland/GAD-Postman/blob/9e9d0264ed60d6d854a2c5320104c23aa351c237/assets/GadPostman_tests.jpg)
