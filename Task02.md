# Kalkulator w JS

1. Napisz kod w JS, który będzie obsługiwał operacje odejmowania, mnożenia, dzielenia w kalkulatorze.

2.  Napisz drugą wersję kalkulatora z wykorzystaniem tylko jednej funkcji, która jako parametr przyjmuje znaki dodawania, odejmowania, mnożenia, dzielenia.

```html
<!DOCTYPE html>
<html lang="pl">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kalkulator Bootstrap</title>
    <!-- Link do arkusza stylów Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
</head>

<body>

    <div class="container mt-5">
        <div class="row">
            <div class="col-md-6 offset-md-3">
                <div class="card">
                    <div class="card-header text-center">
                        Kalkulator
                    </div>
                    <div class="card-body">
                        <form id="calculator-form">
                            <div class="form-group">
                                <input type="number" class="form-control mb-2" id="number1"
                                    placeholder="Pierwsza liczba">
                            </div>
                            <div class="form-group">
                                <input type="number" class="form-control mb-2" id="number2" placeholder="Druga liczba">
                            </div>
                            <div class="text-center">
                                <button type="button" class="btn btn-primary mx-1" onclick="add()">+</button>
                                <button type="button" class="btn btn-primary mx-1" onclick="calculate('-')">-</button>
                                <button type="button" class="btn btn-primary mx-1"
                                    onclick="calculate('*')">&times;</button>
                                <button type="button" class="btn btn-primary mx-1" onclick="calculate('/')">÷</button>
                            </div>
                        </form>
                        <div class="mt-3" id="result"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        function add() {
            let num1 = parseFloat(document.getElementById('number1').value);
            let num2 = parseFloat(document.getElementById('number2').value);

            const result = num1 + num2;

            document.getElementById('result').innerText = 'Wynik: ' + result;
        }
    </script>

</body>

</html>
```
