# Walidacja formularza

1. Dopisz funkcje walidujące pola `Nazwisko` oraz `Adres email`
2. Nazwisko powinno być wypełnione oraz powinno rozpoczynać się z dużej litery - w przypadku negatywnej walidacji pod polem
powinnien pojawić się komunikat o błędzie walidacji.
4. Email powinien być wypełniony oraz zawierać znak `@`- w przypadku negatywnej walidacji pod polem
powinnien pojawić się komunikat o błędzie walidacji.
5. W przypadku ponownego kliknięcia przycisku `Dodaj użytkownika` komunikaty o błędach powinny zostać zresetowane.

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dodaj Użytkownika</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <style type="text/css">
        .errorMsg{
            color:red;
            font-size:12px;
        }
    </style>
</head>
<body>

    <div class="container mt-5">
        <h2>Dodaj nowego użytkownika</h2>
        <form action="#">
            <div class="mb-3">
                <label for="firstName" class="form-label">Imię</label>
                <input type="text" class="form-control" id="firstName">
                <p class="errorMsg" id="userErrorMsg"></p>
            </div>
            <div class="mb-3">
                <label for="lastName" class="form-label">Nazwisko</label>
                <input type="text" class="form-control" id="lastName">
                <p class="errorMsg" id="lastNameErrorMsg"></p>
            </div>
            <div class="mb-3">
                <label for="email" class="form-label">Adres email</label>
                <input type="email" class="form-control" id="email">
                <p class="errorMsg" id="emailErrorMsg"></p>
            </div>
            <button type="button" onclick="validateForm()" class="btn btn-primary">Dodaj użytkownika</button>
        </form>
    </div>
</body>
<script>
    validateForm = () => {

        let validationUser = validateFirstNameInput();

        if (validationUser === false){
            let errorElem = document.getElementById("userErrorMsg");
            errorElem.innerHTML = "Błędna walidacja";
            return;
        }

        alert('formularz zwalidowano');
    }

    function validateFirstNameInput() {
        const username = document.getElementById("firstName").value;
        if (username == null || username.length < 4) {
            return false;
        }
        return true;
    }
</script>

</html>
```
