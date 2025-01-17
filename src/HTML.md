![](https://tva1.sinaimg.cn/large/006y8mN6gy1g87mt8pmwfj3058022744.jpg)



# Curso HTML - JEnPEx 2019

> IFMT Primavera do Leste

## O que é HTML?

HTML não é uma linguagem de programação; é uma *linguagem de marcação* que define a estrutura do seu conteúdo. O HTML consiste em uma série de **[elementos](https://developer.mozilla.org/en-US/docs/Glossary/element)** , que você usa para incluir ou agrupar diferentes partes do conteúdo para que ele apareça de uma certa maneira ou aja de certa maneira. As [tags](https://developer.mozilla.org/en-US/docs/Glossary/tag) anexas podem criar um hiperlink de palavra ou imagem para outro lugar, colocar itálico nas palavras, aumentar ou diminuir a fonte e assim por diante. 

Por exemplo, considere a seguinte linha de conteúdo:

```html
My cat is very grumpy
```

Para inserir esta linha no HTML poderíamos especificar que é um parágrafo colocando-a em tags de parágrafo:

```html
<p>My cat is very grumpy</p>
```

### Anatomia de um elemento HTML

Vamos explorar um pouco mais esse elemento do parágrafo.

![img](https://mdn.mozillademos.org/files/9347/grumpy-cat-small.png)

As principais partes do nosso elemento são as seguintes:

1. **A tag de abertura:** consiste no nome do elemento (neste caso, p), envolto em **colchetes de** abertura e fechamento . Indica onde o elemento começa - nesse caso, onde o parágrafo começa.
2. **A tag de fechamento:** é igual à tag de abertura, exceto pelo fato de incluir uma *barra* antes do nome do elemento. Não adicionar uma tag de fechamento é um dos erros padrão para iniciantes e pode levar a resultados estranhos.
3. **O conteúdo:** este é o conteúdo do elemento, que neste caso, é apenas texto.
4. **O elemento:** a tag de abertura, a tag de fechamento e o conteúdo juntos compõem o elemento.

Além disso, os elementos também podem ter atributos parecidos com os seguintes:

![img](https://mdn.mozillademos.org/files/9345/grumpy-cat-attribute-small.png)

Os atributos contêm informações extras sobre o elemento que você não deseja que apareçam no conteúdo real. Aqui, `class`é o nome do atributo e `editor-note`é o *valor* do atributo . O atributo`class` permite que você atribua ao elemento um identificador que possa ser usado posteriormente para direcionar o elemento com informações de estilo e outras coisas.

Um atributo deve sempre ter o seguinte:

1. Um espaço entre ele e o nome do elemento (ou o atributo anterior, se o elemento já tiver um ou mais atributos).
2. O nome do atributo seguido por um sinal de igual.
3. O valor do atributo envolvido por aspas de abertura e fechamento.

### Aninhamento de elementos

Você também pode colocar elementos dentro de outros elementos - isso é chamado de **aninhamento**. Se quiséssemos afirmar que nosso gato é **muito** mal-humorado, poderíamos envolver a palavra "muito" em um elemento `strong`, o que significa que a palavra deve ser enfatizada fortemente:

```html
<p>My cat is <strong>very</strong> grumpy.</p>
```

No entanto, você precisa garantir que seus elementos estejam aninhados corretamente. No exemplo acima, abrimos o elemento `p`primeiro, depois o elemento `strong`, portanto, temos que fechar o elemento `strong` primeiro, depois o elemento `p`. O seguinte trecho está incorreto:

```html
<p>My cat is <strong>very grumpy.</p></strong>
```

Os elementos precisam abrir e fechar corretamente para que fiquem claramente dentro ou fora um do outro. Se eles se sobreporem, como mostrado acima, seu navegador tentará adivinhar o que você estava tentando dizer, o que pode levar a resultados inesperados. 

> Então não faça isso!

### Elementos vazios

Alguns elementos não têm conteúdo e são chamados de **elementos vazios** . Exemplo disto é o `img`:

```html
<img src="images/firefox-icon.png" alt="My test image">
```

Isso contém dois atributos, mas não há tag de fechamento e conteúdo interno. Isso ocorre porque um elemento de imagem não quebra o conteúdo para afetá-lo. Seu objetivo é incorporar uma imagem na página HTML no local em que aparece.

### Anatomia de um documento HTML

Isso envolve o básico de elementos HTML individuais, mas eles não são úteis por si próprios. Agora, veremos como os elementos individuais são combinados para formar uma página HTML inteira. Vamos revisitar o código que colocamos em nosso `index.html`exemplo (que conhecemos no artigo [Lidando com arquivos](https://developer.mozilla.org/en-US/Learn/Getting_started_with_the_web/Dealing_with_files) ):

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>My test page</title>
  </head>
  <body>
    
  </body>
</html>
```

Aqui, temos o seguinte:

-  `<!DOCTYPE html>`- o doctype. É necessário preâmbulo. Nas brumas do tempo, quando o HTML era jovem (por volta de 1991/92), os doctypes deveriam funcionar como links para um conjunto de regras que a página HTML tinha que seguir para ser considerada um bom HTML, o que poderia significar verificação automática de erros e outras coisas úteis. No entanto, atualmente, eles não fazem muito e são basicamente necessários para garantir que seu documento se comporte corretamente. É tudo o que você precisa saber por enquanto.
- `<html></html>` Esse elemento agrupa todo o conteúdo da página inteira e às vezes é conhecido como elemento raiz.
- `<head></head>` Esse elemento atua como um contêiner para todas as coisas que você deseja incluir na página HTML que *não são* o conteúdo que você está mostrando aos visualizadores da sua página. Isso inclui coisas como [palavras](https://developer.mozilla.org/en-US/docs/Glossary/keyword) - [chave](https://developer.mozilla.org/en-US/docs/Glossary/keyword) e uma descrição da página que você deseja que apareça nos resultados da pesquisa, CSS para estilizar nosso conteúdo, declarações de conjunto de caracteres e muito mais.
- `<meta charset="utf-8">`- define o conjunto de caracteres que seu documento deve usar para UTF-8, que inclui a maioria dos caracteres da grande maioria dos idiomas escritos. Essencialmente, agora ele pode lidar com qualquer conteúdo de texto que você possa colocar nele. Não há razão para não definir isso e isso pode ajudar a evitar alguns problemas mais tarde.
- `<title></title>` define o título da sua página, que é o título que aparece na guia do navegador em que a página é carregada. Também é usado para descrever a página quando você a adiciona aos favoritos / favoritos.
- `<body></body>`contém *todo* o conteúdo que você deseja mostrar aos usuários da Web quando eles visitam sua página, seja texto, imagens, vídeos, jogos, faixas de áudio reproduzíveis ou qualquer outra coisa.

### Elemento Header

O elemento HTML `<header>` inclui informações introdutórias (por exemplo, um título):

```html
...
<body>
	<article>
		<header>
			<h1>JavaScript</h1>
			<h3>O que é JavaScript?</h3>
			<p>Hoje vamos falar sobre JavaScript</p>
		</header>
		<p>JavaScript é uma linguagem de script do lado do cliente usada para prover funcionalidades extras ao usuário</p>
	</article>
</body>
...
```



### Elemento de Divisões

O `<div>`é um elemento HTML em nível de bloco usado para agrupar e organizar páginas da web. Depois de aplicado, os elementos são divididos em seções que você pode formatar usando folha de estilo em cascata (CSS).

```html
<div style="background-color: #333; color: white; padding: 10px;">
  <h3>Título da seção</h3>
  <p>Parágrafo de texto da seção</p>
</div>
```

### Inserindo Imagens

Vamos voltar nossa atenção para o elemento `<img>` novamente:

```html
<img src="https://www.w3.org/html/logo/downloads/HTML5_Badge_512.png" alt="My test image">
```

Como dissemos antes, ele incorpora uma imagem em nossa página na posição em que aparece. Isso é feito através do `src`atributo (source), que contém o caminho para o nosso arquivo de imagem.

Também incluímos um `alt`atributo (alternativo). Nesse atributo, você especifica texto descritivo para usuários que não podem ver a imagem, possivelmente pelos seguintes motivos:

1. Eles são deficientes visuais. Usuários com deficiências visuais significativas geralmente usam ferramentas chamadas leitores de tela para ler o texto alternativo para eles.
2. Algo deu errado, fazendo com que a imagem não fosse exibida. Por exemplo, tente alterar deliberadamente o caminho dentro do seu `src`atributo para torná-lo incorreto. Se você salvar e recarregar a página, deverá ver algo assim no lugar da imagem:

![img](https://mdn.mozillademos.org/files/9349/alt-text-example.png)

## Marcando texto

Esta seção abordará alguns dos elementos HTML essenciais que você usará para marcar o texto.

### Cabeçalhos

Os elementos de cabeçalho permitem especificar que determinadas partes do seu conteúdo são títulos - ou subtítulos. O HTML contém 6 níveis de cabeçalho, `<h1>-<h6>`, embora você normalmente use apenas de 3 a 4 no máximo:

```html
<h1>Titulo Principal</h1>
<h2>Subtítulo</h2>
<h3>Seção</h3>
<h4>Subseção</h4>
```

Agora tente adicionar um título adequado à sua página HTML logo acima da imagem.

> Nota: você verá que seu nível de cabeçalho 1 tem um estilo implícito. Não use elementos de cabeçalho para tornar o texto maior ou em negrito, pois eles são usados para [acessibilidade](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML#Text_content) e outros motivos . Tente criar uma sequência significativa de títulos em suas páginas, sem pular os níveis.

### Parágrafos

Como explicado acima, os elementos `<p>` são para conter parágrafos de texto; você as usará com frequência ao marcar conteúdo de texto comum:

```html
<p>Simples parágrafo de texto</p>
```

Complemente o arquivo adicionando uma descrição logo abaixo da imagem usando a tag `<p>`. 

### Listas

Muito do conteúdo da web é apresentado em listas e o HTML possui elementos especiais para eles. A marcação de listas sempre consiste em pelo menos 2 elementos. Os tipos de lista mais comuns são listas ordenadas e não ordenadas:

1. **Listas não ordenadas** são para listas em que a ordem dos itens não importa, como uma lista de compras. Estes são agrupados em um [``](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)elemento.
2. **As listas ordenadas** são para listas em que a ordem dos itens é importante, como uma receita. Estes são agrupados em um [``](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)elemento.

Cada item dentro das listas é colocado dentro de um elemento [``](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/li)(item da lista).

Por exemplo, se quisermos transformar a parte do fragmento de parágrafo a seguir em uma lista

```html
<p>A programação WEB inclui diferentes tecnologias, sendo as principais o HTML, CSS e o Javascript, que juntas formam poderosas ferramentas para criação de páginas dinâmicas...</p>
```

Poderíamos modificar a marcação para isso

```html
<p>A programação WEB inclui diferentes tecnologias, sendo as principais:</p>
    
<ul> 
  <li>HTML</li>
  <li>CSS</li>
  <li>Javascript</li>
</ul>

<p>que juntas formam poderosas ferramentas para criação de páginas dinâmicas... </p>
```

Tente adicionar uma lista ordenada ou não ordenada à sua página de exemplo.

## Ligações

Os links são muito importantes - são eles que tornam a web uma web! Para adicionar um link, precisamos usar um elemento simples -`<a>`-sendo o "a" o formato abreviado de "ânchora". Para transformar texto em seu parágrafo em um link, siga estas etapas:

1. Escolha algum texto. Nós escolhemos o texto "Mozilla Manifesto".

2. Coloque o texto em um elemento `<a>`, como mostrado abaixo:

   ```html
   <a>Mozilla Manifesto</a>
   ```

3. Adicione o atributo `<href>`ao elemento `<a>`, como mostrado abaixo:

   ```html
   <a href="">Mozilla Manifesto</a>
   ```

4. Preencha o valor desse atributo com o endereço da web ao qual você deseja vincular o link:

   ```html
   <a href="https://www.mozilla.org/en-US/about/manifesto/">Mozilla Manifesto</a>
   ```



Você pode obter resultados inesperados se omitir o `https://`ou `http://`, chamado de *protocolo* , no início do endereço da web. 

Depois de criar um link, clique nele para garantir que ele esteja enviando para onde você deseja.

> O `href`pode parecer uma escolha bastante obscura para um nome de atributo no início. Contudo ele representa **h**ypertext **ref**erence .

Adicione um link à sua página agora, se você ainda não o fez.

## Elementos estruturais

Para simplificar o trabalho com a estrutura do documento para o desenvolvedor, o HTML5 introduziu as tags semânticas:

![](https://tva1.sinaimg.cn/large/006y8mN6gy1g81kc3w2exj3063076mx3.jpg)

- O `header` agrupa as informações de cabeçalho da página

- O `section` organiza as possíveis seções da página.
- O elemento `nav` descreve um espaço especial para **links de navegação** no seu site
- O `article` define uma parte da **informação independente** que pode ser reutilizada
- O `aside` descreve o conteúdo a ser definido ao lado (por exemplo, uma barra lateral)
- O `footer`  define espaço para **notas** de **rodapé**
- Por fim, um elemento que vale a pena destacar é o `main`,  representa o espaço para o **conteúdo principal** de uma página da web.

## Dicas úteis:

Se você não tiver certeza da ordem do seu código, use um **validador HTML** 

- https://validator.w3.org

A lista de todas as tags pode ser encontrada em:

- https://www.w3schools.com/tags/