# Intro.ProgFatec-20211
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Introdução à Programação - Exercício Casa 02</title>
</head>
<body>

    <h1>Exercício 02</h1>
    <p>Solicita o preço do produto e o percentual de desconto.</p>
    
    <form>
        <input id="valor1" type="text" placeholder="Preço do produto">
        <input id="valor2" type="text" placeholder="Percentual de desconto">
        <button id="calcular">Calcular</button>
    </form>

    <script>
        function exemplo() {
            let price = parseFloat(valor1.value)
            let discount = parseFloat(valor2.value)

            let amountDiscounted = price * discount / 100
            let finalPrice = price - amountDiscounted

            document.write(`
            <ul>
                <li>Preço Base: <b>${price}</b>.</li>
                <li>Valor do Desconto: <b>${amountDiscounted}</b>.</li>
                <li>Preço Final: <b>${finalPrice}</b>.</li>
            </ul>           
            `)
        }
        calcular.addEventListener('click', exemplo)

    </script>
</body>
</html>
