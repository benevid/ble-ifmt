![](https://tva1.sinaimg.cn/large/006y8mN6gy1g87mt8pmwfj3058022744.jpg)

# Curso HTML - JEnPEx 2019

> IFMT Primavera do Leste

## JavaScript HTML DOM

Quando uma página da web é carregado, o navegador cria um **D** ocument **O** bject **M** odelo da página.

O **HTML DOM** modelo é construído como uma árvore de **objetos** :

![DOM HTML tree](https://www.w3schools.com/js/pic_htmltree.gif)

Com o modelo de objeto, JavaScript recebe toda a energia de que necessita para criar HTML dinâmico:

- JavaScript pode mudar todos os elementos HTML na página
- JavaScript pode mudar todos os atributos HTML na página
- JavaScript pode mudar todos os estilos CSS na página
- JavaScript pode remover elementos HTML e atributos existentes
- JavaScript pode adicionar novos elementos e atributos HTML
- JavaScript pode reagir a todos os eventos HTML existentes na página
- JavaScript pode criar novos eventos HTML na página

## Qual é o DOM?

O DOM é um padrão W3C (World Wide Web Consortium).

O DOM define um padrão para acessar os documentos:

*"O modelo de objeto de W3C DOM (Document) é uma interface de plataforma e de linguagem neutra que permite que programas e scripts para acessar e atualizar o conteúdo, estrutura e estilo de um documento dinamicamente."*

O padrão W3C DOM é separada em 3 partes diferentes:

- DOM núcleo - modelo padrão para todos os tipos de documentos
- DOM XML - modelo padrão para documentos XML
- HTML DOM - modelo padrão para documentos HTML

------

## Qual é o DOM HTML?

O HTML DOM é um padrão **objeto** modelo e **interface de programação** de HTML. Ele define:

- Os elementos HTML como **objetos**
- As **propriedades** de todos os elementos HTML
- Os **métodos** para acessar todos os elementos HTML
- Os **eventos** para todos os elementos HTML

Em outras palavras: **O HTML DOM é um padrão para como obter, alterar, adicionar ou excluir elementos HTML.**



## A interface de programação DOM

O DOM HTML pode ser acessado com JavaScript (e com outras linguagens de programação).

No DOM, todos os elementos HTML são definidos como **objetos** .

A interface de programação é as propriedades e métodos de cada objecto.

A **propriedade** é um valor que você pode obter ou conjunto (como alterar o conteúdo de um elemento HTML).

Um **método** é uma ação que você pode fazer (como adicionar ou excluir um elemento HTML).

```html
<html>
<body>

<p id="demo"></p>

<script>
	document.getElementById("demo").innerHTML = "Hello World!";
</script>

</body>
</html>
```

No exemplo acima, `getElementById`é um **método** , enquanto que `innerHTML`é uma **propriedade** . A `innerHTML`é útil para obter ou substituir o conteúdo de elementos HTML.

### Buscando Elementos HTML

| Method                                  | Description                   |
| :-------------------------------------- | :---------------------------- |
| document.getElementById(*id*)           | Find an element by element id |
| document.getElementsByTagName(*name*)   | Find elements by tag name     |
| document.getElementsByClassName(*name*) | Find elements by class name   |

### Mudando elementos

| Property                                   | Description                                   |
| :----------------------------------------- | :-------------------------------------------- |
| *element*.innerHTML = *new html content*   | Change the inner HTML of an element           |
| *element*.*attribute = new value*          | Change the attribute value of an HTML element |
| *element*.style.*property = new style*     | Change the style of an HTML element           |
| Method                                     | Description                                   |
| *element*.setAttribute*(attribute, value)* | Change the attribute value of an HTML element |

### Adicionar e eliminar Elements

| Method                            | Description                       |
| :-------------------------------- | :-------------------------------- |
| document.createElement(*element*) | Create an HTML element            |
| document.removeChild(*element*)   | Remove an HTML element            |
| document.appendChild(*element*)   | Add an HTML element               |
| document.replaceChild(*new, old*) | Replace an HTML element           |
| document.write(*text*)            | Write into the HTML output stream |

### Adicionando Eventos Manipuladores

| Method                                                     | Description |
| :--------------------------------------------------------- | :---------- |
| document.getElementById(*id*).onclick = function(){*code*} |             |

## Alterar o valor de um atributo

Para alterar o valor de um atributo HTML, use esta sintaxe:

document.getElementById(*id*).*attribute = new value*

Este exemplo altera o valor do atributo src de um elemento `<img>`:

```html
<!DOCTYPE html>
<html>
<body>

<img id="myImage" src="smiley.gif">

<script>
document.getElementById("myImage").src = "landscape.jpg";
</script>

</body>
</html>
```

## Criar a animação usando JavaScript

Animações em JavaScript são feitas através da programação mudanças graduais em estilo de um elemento.

```html
<!DOCTYPE html>
<html>
<style>
#container {
  width: 400px;
  height: 400px;
  position: relative;
  background: yellow;
}
#animate {
  width: 50px;
  height: 50px;
  position: absolute;
  background-color: red;
}
</style>
<body>

<p><button onclick="myMove()">Click Me</button></p> 

<div id ="container">
  <div id ="animate"></div>
</div>

<script>
function myMove() {
  var elem = document.getElementById("animate");   
  var pos = 0;
  var id = setInterval(frame, 5);
  function frame() {
    if (pos == 350) {
      clearInterval(id);
    } else {
      pos++; 
      elem.style.top = pos + "px"; 
      elem.style.left = pos + "px"; 
    }
  }
}
</script>

</body>
</html>
```

## Reagindo a eventos

A JavaScript pode ser executado quando um evento ocorre, como quando um usuário clica em um elemento HTML.

Exemplos de eventos de HTML:

- Quando um usuário clica o mouse
- Quando uma página web foi carregado
- Quando uma imagem tiver sido carregado
- Quando o rato se move ao longo de um elemento
- Quando um campo de entrada for alterado
- Quando um formulário HTML é submetido
- Quando um usuário acaricia uma chave

Para executar código quando um usuário clica em um elemento, adicionar um código JavaScript para um atributo do evento HTML:

```html
<!DOCTYPE html>
<html>
<body>

<h1 onclick="this.innerHTML = 'Ooops!'">Click on this text!</h1>

</body>
</html>
```

Para atribuir eventos a elementos HTML você pode usar atributos de eventos.

```html
<!DOCTYPE html>
<html>
<body>

<p>Click "Try it" to execute the displayDate() function.</p>

<button id="myBtn">Try it</button>

<p id="demo"></p>

<script>
document.getElementById("myBtn").onclick = displayDate;
//document.getElementById("myBtn").addEventListener("click", displayDate);
function displayDate() {
  document.getElementById("demo").innerHTML = Date();
}
</script>

</body>
</html> 

```

## Modelo Padrão

Acessando um objeto JSON usando anotações:

```html
<!DOCTYPE html>
<html>
<body>

<p>Access a JSON object using dot notation:</p>

<p id="demo"></p>

<script>
var myObj, x;
myObj = {"name":"John", "age":30, "car":null};
x = myObj.name;
document.getElementById("demo").innerHTML = x;
</script>

</body>
</html>
```



