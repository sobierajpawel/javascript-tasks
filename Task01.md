# Obsługa funkcji i manipulacja elementami

1. Napisz funkcje obsługujące przyciski:
  - `enterText()` wprowadza dowolny tekst w pole `input`
  - `changeColor()` - zmienia kolor stopki na dowolny
  - `showAlert()` - pokazuje alert dialogowy z dowolnym teskterm
  - `showConsole()` - wyświetli tekst w konsoli

```html
<!DOCTYPE html>
<html lang="pl">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formularz Bootstrap</title>
  <!-- Link do arkusza stylów Bootstrap CSS -->
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>

<body>

  <div class="container mt-5">
    <div class="row">
      <div class="col-md-8 offset-md-2">
        <div class="card">
          <div class="card-body">
            <form id="action-form">
              <div class="mb-3">
                <input type="text" class="form-control" id="inputText" placeholder="Wpisz jakiś tekst">
              </div>
              <button type="button" class="btn btn-primary" onclick="enterText()">Wprowadź przykładowy tekst</button>
              <button type="button" class="btn btn-secondary" onclick="changeColor()">Zmień kolor</button>
              <button type="button" class="btn btn-info" onclick="showAlert()">Pokaż dialog</button>
              <button type="button" class="btn btn-info" onclick="showConsole()">Wyświetl w konsoli</button>
            </form>
          </div>
          <div class="card-footer" id="colorChangeable">
            Tekst zmieniający kolor
          </div>
        </div>
      </div>
    </div>
  </div>
</body>
<script>
</script>
</html>
```
