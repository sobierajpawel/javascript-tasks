# jQuery

1. Napisz przy wykorzystaniu jQuery metody do obsługi kliknięcia w dostępne przyciski.
2. Zgodnie z opisem funkcje po kliknięciu powinny odpowiednio zmieniać styl pola `input`, dodawać przykładowy tekst, chować, pokazywać element (możesz skorzystać z funkcji `slideUp` oraz `slideDown`)
```html
<!DOCTYPE html>
<html>

<head>
    <title>Ćwiczenie jQuery</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>

<body>
    <div class="container mt-5">
        <div class="row">
            <div class="col-md-9 offset-md-2">
                <div class="card">
                    <div class="card-header text-center">
                        jQuery
                    </div>
                    <div class="card-body">
                        <div class="form-group">
                            <input type="text" id="textInput" placeholder="Twój tekst" class="form-control" />
                        </div>
                        <div class="form-group">
                            <button class="btn btn-primary" id="styleText">Zmień styl input'a</button>
                            <button class="btn btn-warning" id="fillText">Wypełnij Tekst</button>
                            <button class="btn btn-danger" id="showMessage">Pokaż Komunikat</button>
                            <button class="btn btn-success" id="hideMessage">Ukryj Komunikat</button>
                        </div>
                        <div class="form-group">
                            <div id="message"
                                style="display: none; margin-top: 10px; border: 1px solid red; padding: 5px;">
                                Komunikat: Tekst został wypełniony!
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
    <script>
    </script>
</body>
</html>
```
