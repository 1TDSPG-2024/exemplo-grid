# O que é o CSS Grid Layout?

O CSS Grid Layout é um sistema de layout bidimensional que permite criar layouts complexos e flexíveis em páginas da web de uma maneira mais intuitiva e eficiente. Ele introduz uma grade (ou grid) para organizar elementos em linhas e colunas, oferecendo controle preciso sobre a posição e o dimensionamento desses elementos.

## Conceitos-chave do CSS Grid Layout:

- **Grid Container**: Um elemento HTML que é definido como um grid container usando `display: grid;`. Ele contém todos os elementos que formam o grid.

- **Grid Items**: Os elementos filhos diretos de um grid container são chamados de grid items. Eles são posicionados dentro das células da grade.

- **Grid Lines**: As linhas horizontais e verticais que definem a estrutura da grade são chamadas de grid lines. Elas dividem a área da grade em células.

- **Grid Tracks**: As linhas ou colunas entre quaisquer duas linhas ou colunas adjacentes são chamadas de grid tracks. Elas podem ser dimensionadas para determinar a largura ou a altura das células da grade.

- **Grid Cells**: Os espaços retangulares formados pela interseção de linhas adjacentes são chamados de grid cells. Cada grid cell pode conter um ou mais grid items.

- **Grid Areas**: Regiões retangulares na grade que podem conter um ou mais grid items são chamadas de grid areas. Elas são definidas atribuindo nomes às células da grade.

[O CSS Grid Layout oferece recursos poderosos, como alinhamento flexível de conteúdo, controle preciso sobre a posição dos itens e facilidade de criar layouts responsivos. Ele complementa outras técnicas de layout em CSS, como Flexbox, e é especialmente útil para criar layouts complexos, como layouts de grade de revistas ou layouts de painéis e de administração.]

# Exemplo de CSS Grid Layout

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemplo de CSS Grid Layout</title>
    <style>
        .container {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 10px;
            background-color: #f0f0f0;
            padding: 20px;
        }

        .item {
            background-color: #ccc;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Item 5</div>
        <div class="item">Item 6</div>
    </div>
</body>
</html>


Esse exemplo cria uma grade com três colunas, onde cada coluna tem a mesma
largura (`1fr`). Os itens dentro da grade são divs com a classe `.item`.
O CSS define estilos para a `.container` como uma grade com espaçamento 
entre as células e estilos básicos para os itens.
