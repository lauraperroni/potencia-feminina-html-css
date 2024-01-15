# Anotações do Curso de HTML e CSS da Potência Feminina MaisMulheres.tech
Anotações feitas pela aluna Laura Perroni, de Viamão - Rio Grande do Sul

Fiquem à vontade para adicionar, alterar, melhorar este arquivo! <3

## MÓDULO 1 - Introdução 

#### HTML
É a linguagem para marcação de hipertextos
Baseado na SGML
Teve várias versões, está na HTML5

##### Links úteis: 

[Projeto do curso no Github](https://github.com/WoMakersCode/html-css-womakerscode-irme)

[Site W3C](https://www.w3.org/)

[Site Can I Use?](https://caniuse.com/)

[Google Chrome](https://www.google.com/intl/pt-BR/chrome/)

[Visual Studio Code](https://code.visualstudio.com/?WT.mc_id=javascript-12143-gllemos)

[Visual Studio Live Server](http://bit.ly/2VqzdzT)

## MÓDULO 2 - Conhecendo o HTML 

#### Estrutura do HTML

```
<p>Exemplo de tag.</p>
<p>Exemplo de tag<em> em aninhamento</em>.</p>
<p class="exemplo">Exemplo de atributo</p>
```

#### Tags e atributos

* ```<!DOCTYPE html>``` => indica a versão do html
* ```<html>```  => contém os elementos da página toda
* ```<head>```  => parte invisível da página como cabeçalho, título, caracteres, etc...
* ```<meta charset="UTF-8">``` => caracteres utilizados na página
* ```<title>```  => título da página (na aba)
* ```<body>```  => corpo da página, conteúdo visível do site
* ```<p>``` => parágrafo de texto
* ```<h1>```  => título de texto, vai do h1 até o h6 em ordem decrescente
* ```<html lang="pt-br">```  =>  indica o idioma da página
* ```<meta name="author" content="laura">``` => indica o autor da página
* ```<em>``` => enfatiza uma palavra no texto em itálico
* ```<strong>``` => enfatiza uma palavra no texto em negrito

#### Outras tags importantes
* ```<header>``` => cabeçalho da página (logotipo, título, menu de navegação, etc...) 
* ``````<nav>``` => indica a navegação no site ou página
* ```<main>``` => conteúdo principal da página, aparece só 1x
* ``````<nav>``` => indica a navegação no site ou página
* ```<footer>``` => rodapé da página
* ```<nav>``` => indica a navegação no site ou página
* ```<aside>``` => conteúdo relacionado ao main da página
* ```<article>``` => conteúdos independentes ou reutilizáveis/blogs
* ```<section>``` => uma seção da página/cabeçalho + texto
* ```<div>``` => tag genérica, agrupa elementos
* ```<span>``` =>  igual a uma div, mas para estilizar textos

##### Links úteis: 

**ARTIGO**  [Elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element)

**ARTIGO**  [Atributos HTML](https://developer.mozilla.org/pt-BR/docs/HTML/Attributes)

**ARTIGO**  [Meta Informações](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/meta)

**ARTIGO**  [Elementos HTML de conteúdo textual](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element#conte%C3%BAdo_textual)

**ARTIGO**  [Semânticas textuais inline](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element#sem%C3%A2nticas_textuais_inline)

**ARTIGO**  [Criando hyperlinks](https://developer.mozilla.org/pt-BR/docs/Aprender/HTML/Introducao_ao_HTML/Criando_hyperlinks)

**ARTIGO**  [Formulários em HTML](https://developer.mozilla.org/pt-BR/docs/Web/Guide/HTML/Forms)

**ARTIGO**  [Trabalhando com Botões](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/button)

**ARTIGO**  [Conteúdos Multimídia e Embutidos na página](https://developer.mozilla.org/pt-BR/docs/Aprender/HTML/Multimedia_and_embedding)

**ARTIGO**  [Tabelas em HTML](https://developer.mozilla.org/pt-BR/docs/Aprender/HTML/Tables)

## MÓDULO 3 - HTML além do óbvio 

#### H1
Só devemos utilizar 1 h1 em cada página, e manter uma hierarquia entre os "h"s.

#### Listas

**Lista ordenada:**

```
<ol> 
	<li>Item 1</li>
	<li>Item 2</li>
	<li>Item 3</li>
</ol>
```

**Lista não ordenada**

```
<ol> 
	<li>Item 1</li>
	<li>Item 2</li>
	<li>Item 3</li>
</ol>
```
#### Links

```<a href="link">Clique aqui</a>```  Coloca link em um texto dentro do <a>


```<a href="link" title="o maior site de buscas" target="_blank" rel="noreferrer">Clique aqui</a>``` Abre link de um texto em uma nova aba do navegador (target), não permite que a aba nova acesse a sua(rel), e tem um título ao hover(title.)


#### Formulários

```
<form>
	<div>   
		<labelfor="name" placeholder="seu nome completo">Nome completo</label>
		<input type="text" id="nome"> 
	</div>
	<div>   
		<labelfor="descricao">Descrição do problema</label>
		<textarea></textarea> 
	</div>
	<button type="submit">Enviar mensagem</button>
</form>
```

#### Multimidia

```
<figure>
	<img src="img/gato.png" alt="foto de gato" title="foto gato">
	<fgcaption>Gato fofo e engraçado</figcaption>
</figure>
```
Se a foto for só de decoração do site, deixamos seu alt assim: alt=""

#### Tabelas

```
<table>
	<caption>Datas de aniversário</caption>
	<tr>
		<td>Nome</td>
		<td>Idade</td>
	</tr>
	<tr>
		<td>Laura</td>
		<td>22</td>
	</tr>
</table>
```

#### Gerenciamento de foco

O atributo tabindex informa ao navegador qual a ordem de foco dos elementos da página.
Foco = quando apertamos tab no teclado, a página foca em algum elemento.

```<div tabindex="1"></div>``` Retira focos ou modifica a ordem dos elementos

#### Aria Properties, Roles and States


```
<form role="search></form>
<button aria_haspopup="true"></button>
<input type="checkbox" aria_selected="true">
```


##### Links úteis: 

**ARTIGO** [Guia WCAG](https://guia-wcag.com/)

**ARTIGO** [Papéis/Funções ARIA](https://developer.mozilla.org/pt-BR/docs/Web/Accessibility/ARIA/ARIA_Techniques#fun%C3%A7%C3%B5es)

**ARTIGO** [Estados e Propriedades ARIA](https://developer.mozilla.org/pt-BR/docs/Web/Accessibility/ARIA/ARIA_Techniques#estados_e_propriedades)

**ARTIGO** [Acessibilidade no HTML](https://developer.mozilla.org/pt-BR/docs/Learn/Accessibility/HTML)

**ARTIGO** [3 Ferramentas para avaliar a acessibilidade web](https://medium.com/bruno-pulis/3-ferramentas-para-avaliar-a-acessibilidade-web-41fa8091e42b)

## MÓDULO 4 - Introdução ao CSS 

Folha de estilo em cascata
Tem do CSS1 até o atual, CSS3

#### Forma inline

Quando escrevemos o CSS direto em algum elemento do próprio HTML
Exemplo:

```
<p style="color: blue;">Essa é a forma inline</p>
```

#### Forma interna

Quando colocamos a configuração para certos elementos no HTML. 
Exemplo:

```
<style>
	p {
		color: red;
	}
</style>
```

#### Forma externa

Quando temos um arquivo de estilo .css que configure nosso HTML.
Exemplo:

**No HTML**
```
<p>Esse é um parágrafo</p>
```

**No CSS**
```
p {
	color: red;
}
```


#### Principais Seletores CSS

* class => apelido para um elemento
* id => identificador único de um elemento
* * => seletor global, é para todos os elementos
* main h2 => pega o elemento dentro da tag main e seus colegas


#### Principais Pseudo-Seletores CSS

* .exemplo:hover => regra para quando o cursos passa por cima do elemento
* .exemplo:focus => regra para quando o elemento está em foco
* .exemplo:active => regra para quando o elemento é clicado ou pressionado
* .li:first-child => regra para o primeiro elemento de uma lista
* .li:last-child => regra para o último elemento de uma lista
* .li:nth-child(1) => regra para o elemento de uma lista na posição informada

#### Principais Pseudo-Elementos CSS

* .classe::after => coloca o conteúdo filho após um elemento
* .classe::before => coloca o conteúdo filho antes de um elemento

##### Links úteis: 

**ARTIGO** [Seletores CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Selectors)

**JOGO** [CSS Diner](https://flukeout.github.io/)

**ARTIGO** [Pseudo-classes para seleção de elementos](https://developer.mozilla.org/pt-BR/docs/Web/CSS/Pseudo-classes)

**ARTIGO** [Usando pseudo-elementos como seletores](https://developer.mozilla.org/pt-BR/docs/Web/CSS/Pseudo-elementos)

## MÓDULO 5 - Entendendo unidades de medida e cores 


#### Cores

```
	.exemplo {
		color: red;
		color: rgb(0, 0, 0);
		color: #00ff00
	}
```

#### Unidades de Medida

```
	.exemplo {
		width: 150px;
		height: 150px;
	}
```

#### Definições de Display

##### Links úteis: 

**ARTIGO** [Trabalhando com cores no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/color_value)

**ARTIGO** [Guia de Unidades no CSS](https://www.alura.com.br/artigos/guia-de-unidades-no-css)

**ARTIGO** [Um guia completo de tipografia para a web](https://tableless.com.br/um-guia-completo-de-tipografia-para-a-web/)

**ARTIGO** [Entendendo o font-family](https://developer.mozilla.org/pt-BR/docs/Web/CSS/font-family)

## MÓDULO 6 - Posicionando os elementos na página 

##### Links úteis: 

**ARTIGO** [Propriedade display no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/display)

**ARTIGO** [Propriedade position no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/position)

**ARTIGO** [Entendendo o box model](https://developer.mozilla.org/pt-BR/docs/Web/CSS/box_model)


## MÓDULO 7 - Conhecendo as propriedades CSS 

##### Links úteis: 

**ARTIGO** [Propriedade border no CSS](https://developer.mozilla.org/pt-PT/docs/Web/CSS/border)

**ARTIGO** [Propriedade border-radius no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/border-radius)

**ARTIGO** [Propriedade box-shadow no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/box-shadow)

**ARTIGO** [Propriedade cursor no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/cursor)

**ARTIGO** [Propriedade outline no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/outline)

**ARTIGO** [A importância do foco visível para a acessibilidade digital](https://uxdesign.blog.br/a-import%C3%A2ncia-do-foco-vis%C3%ADvel-para-a-acessibilidade-digital-5838466f08b5)

**ARTIGO** [Propriedade float no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/float)

**ARTIGO** [Propriedade overflow no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/overflow)

**ARTIGO** [Propriedade font-size no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/font-size)

**ARTIGO** [Propriedade font-weight no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/font-weight)

**ARTIGO** [Propriedade text-align no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/text-align)

**ARTIGO** [Propriedade text-indent no CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/text-indent)

**ARTIGO** [Propriedade letter-spacing no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/letter-spacing)

**ARTIGO** [Propriedade line-height no CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height)

**ARTIGO** [Propriedade list-style no CSS](https://developer.mozilla.org/pt-PT/docs/Web/CSS/list-style)

**ARTIGO** [Propriedade text-decoration no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/text-decoration)

**ARTIGO** [Propriedade background no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/background)

**ARTIGO** [Referências de CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Reference)

## MÓDULO 8 - Principais conceitos do CSS 

##### Links úteis: 

**ARTIGO** [Como usar herança no CSS?](https://tableless.com.br/afinal-como-usar-heranca-no-css/)

## MÓDULO 9 - Animações com CSS 

##### Links úteis:
 
**ARTIGO** [Trabalhando com transições no CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)

**ARTIGO** [Trabalhando com animações no CSS](https://codepen.io/afonsopacifer/post/hora-de-aventura-com-css-5-animacoes)


## MÓDULO 10 - Transformações com Layouts 

## Definições de display 

O display none esconde o elemento
Top, Bottom, Left e Right indicam a distancia do element em relação ao topo, baixo, esquerda e direita.

	O position absolute fica por cima e ignora qualquer elemento
	O position static é estático
	O position relative fica posicionado em relação ao que indicamos
	O z-index especifica a ordem que um elemento e seus filhos aparecem na tela no eixo z
	O position fixed se comporta como o absolute, mas fica fixo na página, se rolar a caixa vai junto.
	
## Definindo espaçamentos para elementos 

	margin   é a margem do elemento. 
	margin-top, margin-left, margin-right, margin-bottom.
	margin: 5px 10px 15px 20px
	margin: 30px 40px -> direita + esquerda são 40/ cima e baixo são 30
		padding   define o espaçamento interno dos elementos 
	
## Propriedades genéricas 

	border - adiciona borda ao elemento
		width, style, color, radius, 
	box-shaddow - coloca sombra no elemento
	cursor - coisas que aparecem ao passar o mouse por cima
	outline - controla a borda dos elementos
	float - troca o fluxo do posicionamento do elemento
	overflow - diz o que acontece com o conteúdo que sai da caixa]
		scroll, hidden.
	
## Propriedades de texto 
		
	font-size   controla o tamanho dos textos
	font weight   peso da fonte, pode ser numero ou bols
	text-align   alinhamento do conteúdo 
	text-indent   define o espaço antes de uma linha de texto
	letter-spacing   espaçamento entre as letras do elemento
	lign-height   altura da linha de texto
	
## Propriedades de listas 

	list-style   dá o estilo do marcador da lista
		none, square, lower-roman, 
		
## Propriedades de links                          
	
	text-decoration: tira o sublinhado do link
	link:hover   quando passa em cima do link
	<a href "#"   leva a lugar nenhum
	.link:active   quando estiver focado/clicado
	
## Propriedades de outras coisas 
	
	background-image   coloca imagem no background do elemento
	background-repeat   repete ou não a imagem no elemento
	backgroud-position   diz a posição da imagem
	background-siza   diz o tamanho da imagem
	
	
## O efeito cascata no CSS 
	
As regras que estiverem mais abaixo se sobrepõe sobre as 
regras que estão mais em cima, por conta do efeito cascata.
	
	
## Herança do CSS 
	
Alguns estilos passam de pai para filho no CSS, como por exemplo uma section que tem um div dentro e seu estilo definido no CSS.
Não se passam propriedades de box model (height, width, background-color, etc...
Pode-se forçar a herança por meio do inherit.
	
	
## Calculo de especificidade 
	
Entender que seletores diferentes tem pesos diferentes
independente da cascata.
Classes tem mais peso que um seletor genérico como P
Quanto mais específico, mais prioridade tem no CSS
Se for colocado inline, terá prioridade também.
	
## Animações com CSS 
	```
	transition: background-color 0.5s   diz quanto tempo leva para trocar a cor
	```
## Animações com uma linha do tempo 

Exemplo:
	```
	@keyframes animacao {
		0% {
			background-color: blue;
		}
		100% {
			background-color: pink;
		}
	}
	
	.caixa {            <- vai fazer a animação girar infinitamente
	width: 50px;
	height: 50px;
	animation: animacao 1s infinite; (alternate, etc...)
	}
	```
## Performance em animações 
	
É a velocidade do computador em calcular tudo da página
	
Para melhorar performance usamos o will-change e passamos os valores que irão mudar.

## Trabalhando com Scale 
	
Usado para transformar a escala do elemento, utilizando proporção
Exemplo: 
	```
	.caixa {
	width: 100px;
	height: 100px;
	background-color: blue;
	transform: scale(2);
	}
	```
	
## Trabalhando com rotate              
	
Rotaciona o elemento.
Exemplo: 
	```
	.caixa {
	width: 100px;
	height: 100px;
	background-color: blue;
	animation: girando 2s infinite;
	}

	@keyframes girando {
		0% {
			transform: rotate(0deg);
		}
		100% {
			transform: rotate(360deg);
		}
	}
	```
## Trabalhando com translate              

Para transformar a posição dos elementos, utilizamos o translate
Exemplo: 
	```
	.caixa {
	width: 100px;
	height: 100px;
	background-color: blue;
	transform: translate(30px, 30px);  -> horizontal e vertical
	}
	```
## Trabalhando com Skew                 
	
o Skew é usado para distorcer os elementos, tipo entortar eles.
Exemplo: 
	```
	.caixa {
	width: 100px;
	height: 100px;
	background-color: blue;
	transform: skewX(10deg);
	}
	```

## Trabalhando com opacity              

Transforma a opacidade de um elemento.
Exemplo: 
	```
	.botao {
		opacity: .5;
	}
	```
## Entendendo o Box Model                

Box model é tudo que influencia o tamanho final do elemento.
Exemplo: 
	```
	.caixa {
	width: 100px;
	height: 100px;
	background: pink;
	padding: 10px;
	border: 5px solid green;
	box-sizing:  border-box;
	margin: 10px;
	}
	```
## MÓDULO 11 - Trabalhando com Layouts                   
	
### Introdução ao Flexbox

Exemplo: 
	```
	.container {
		border: 1px solid green;
		display: inline-flex;
	}
	.caixa {
		background: pink;
		width: 50px;
		height: 50px;
		border 1px solid blue;
	}
	```
#### Flex-direction

Podemos controlar a direção dos flex-itens com o flex-direction
Row é o valor padrão, temos:
-Row, row-reverse, column, column-reverse etc...
Exemplo:  
	```
	.container {
		border: 1px solid green;
		display: flex;
		flex-direction: row;
	}
	.caixa {
		background: pink;
		width: 50px;
		height: 50px;
		border 1px solid blue;
	}
	```
#### Flex-wrapping

Indica como os elementos vão se comportar quando a tela aumentar ou diminuir
Pode ser: wrap, no-wrap
Exemplo: 
	```
	.container {
		border: 1px solid green;
		display: flex;
		flex-wrapping: wrap;
	}
	.caixa {
		background: pink;
		width: 50px;
		height: 50px;
		border 1px solid blue;
	}
	```
#### Flex-flow 

Funciona como um shorthand/substituto para as propriedades flex-direction e flex-wrapping, passando duas informações.
Exemplo: 
	```
	.container {
		border: 1px solid green;
		display: flex;
		flex-flow: row-reverse wrap;
	}
	.caixa {
		background: pink;
		width: 50px;
		height: 50px;
		border 1px solid blue;
	}
	```
#### Justify-content

Nos permite alinhar os flex-itens horizontalmente.
Só funciona com elementos de uma linha só, e também não funciona caso o flex-wrapping seja wrap.
Pode ser:  flex-start (à esquerda), flex-end(à direita),  center(ao centro), space-between(coloca espaço igual 
entre itens), space-around(coloca espaço à direita e à esquerda dos itens), space-evenly(espaços iguais nos vãos dos itens).
Exemplo: 
	```
	.container {
		border: 1px solid green;
		display: flex;
		justify-content: space-around;
	}
	.caixa {
		background: pink;
		width: 50px;
		height: 50px;
		border 1px solid blue;
	}
	```
#### Align-items

Resolve o alinhamento vertical dos itens.

Pode ser: flex-start(no topo, de acordo com conteudo),
flex-end(em baixo, por conteúdo), center(no centro, por 
conteúdo.)
Exemplo: 
	```
	.container {
		border: 1px solid green;
		display: flex;
		align-items: flex-start;
	}
	.caixa {
		background: pink;
		width: 50px;
		height: 50px;
		border 1px solid blue;
	}
	```
#### Align-content

Alinha os flex-itens em flex-containers e permite mais de uma linha
É quase igual ao align-items, mas permite que tenha mais de uma linha
Pode ser: stretch(estica o conteudo), flex-start(altura por conteúdo, 
no topo do flex-container), flex-end (na parte de baixo, por conteúdo),
center(no centro, por conteúdo), space-between(verticalmente, alinha à
parte de baixo.) space-around(alinhamento vertical com espaço em volta),


Exemplo:
	```
  	.container {
		border: 1px solid green;
		display: flex;
		width: 50px;
		height: 50px;
		flex-wrap: wrap;
		align-content: stretch;
	}
	.caixa {
		background: pink;
		width: 50px;
		height: 50px;
		border 1px solid blue;
	}
	```
#### Order

A propriedade order é utilizada nos flex-items para alterar a ordem na
qual eles são exibidos no flex-container.

Exemplo:
	```
	.caixa:nth-child(1) {
		order: 1;
	}
	
	.caixa:nth-child(2) {
		order: 2;
	}
	
	.caixa:nth-child(3) {
		order: 3;
	}
	```
#### Flex-grow

Define o poder de um flex-item de aumentar de tamanho se necessário.
Se colocar o mesmo flex-grow para todos os itens de um container, eles
irão se ajustar e aumentar de acordo.
Por exemplo, se passarmos 2 para um dos elementos, ele passará a ocupar o dobro de 
espaço que os outros elementos estão ocupando.

Exemplo:
	```
	.caixa:nth-child(1) {
		flex-grow: 1;
	}
	
	.caixa:nth-child(2) {
		flex-grow: 1;
	}
	
	.caixa:nth-child(3) {
		flex-grow: 1;
	}
	```
#### Flex-shrink

Determina como um flex-item vai se contrair/shrink.
Se colocar 0, o item não irá diminuir quando a tela diminuir, apenas
os outros itens diminuirão.
Se colocar algum número maior que 1, o item irá diminuir mais rápido
que os outros itens.

Exemplo:
	```
	.caixa:nth-child(1) {
		flex-shrink: 0;
	}
	```
#### Flex-basis

Define o tamanho inicial do flex-item, independente do container.


Exemplo: 
	```
	.caixa {
	background: pink;
	width: 70px;
	height: 70px;
	border: 1px solid blue;
	}
	
	.caixa:nth-child(1) {
		flex-basis: 100px;
	}
	```
#### Flex

É uma abreviação das propriedades flex-grow, flex-shrink e flex-basis.

Exemplo:
	```
	.caixa {
	background: pink;
	width: 70px;
	height: 70px;
	border: 1px solid blue;
	}
	
	.caixa:nth-child(1) {
		flex: 0 1 100px;   -> declara os 3 em um só.
	}
	```
#### Align-Self

Permite que um flex item se posicione verticalmente independente do seu flex-container.
Aceita todos os valores que a align-items aceita.

Exemplo: 
	```
	.caixa {
	background: pink;
	width: 70px;
	height: 70px;
	border: 1px solid blue;
	}
	
	.caixa:nth-child(1) {
		align-self: flex-end;
	}
	```
### Introdução ao Grid-Layout no css

Famoso para construir layouts. 
Trabalha de forma bidimensional, com linhas E colunas.

Exemplo: 
```
	.container {
		border: 2px solid green;
		display: grid;
		grid-template-columns: 100px 100px 50px; <- 3 colunas com esses tamanhos
		grid-gap: 10px <- espaço entre uma coluna e outra
	}
	```
	```
	.caixa {
		background: pink;
		padding: 20px;
	}
	```
### Outras especificações de Layout 

#### Multi-column Layout
Exemplo:
	```
	.colunas {
	column-count: 2;
	}
	```
	
##### Links úteis: 

Acesse os links abaixo:

**ARTIGO** [Box model para iniciantes](https://tableless.github.io/iniciantes/manual/css/box-model.html)

**ARTIGO** [Trabalhando com Flexbox](https://codepen.io/afonsopacifer/post/hora-de-aventura-com-css-9-flexbox)

**ARTIGO** [Conceitos básicos do Flexbox](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Flexible_Box_Layout/Conceitos_Basicos_do_Flexbox)

**ARTIGO** [Guia completo Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

**JOGO** [Flexbox Froggy](https://flexboxfroggy.com/)

**ARTIGO** [Conceitos básicos de Grid Layout](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Grid_Layout/Basic_Concepts_of_Grid_Layout)

**ARTIGO** [Entendendo o CSS Grid Layout](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Grid_Layout)

**ARTIGO** [Guia completo Grid Layout](https://css-tricks.com/snippets/css/complete-guide-grid/)

**JOGO** [CSS Grid Garden](https://cssgridgarden.com/)

**ARTIGO** [CSS Grid e Flexbox - Quando utilizar?](https://www.felipefialho.com/blog/css-grid-e-flexbox-quando-utilizar/)


## MÓDULO 12 - Trabalhando com responsividade

#### O que é responsividade
Um conjunto de técnicas que permite que um mesmo site se adapte a diversos tamanhos de tela diferentes.
Um site responsivo é um site que se adapta facilmente a qualquer tamanho de tela.
Devemos garantir que nosso site seja responsivo, independente do tamanho de tela.
Exemplo: 

	[Site do Netflix](https://netflix.com)

#### Trabalhando com media queries
Media Queries servem para criar regras que se aplicam a diferentes tamanhos de tela.

Exemplo: 
```	
	.caixa {
		width: 300px;
		height: 300px;
		background-color: green;
	}
```
```	
	@media (max-width: 600px) {
		.caixa { 
			background-color: pink;
		}
```
Nesse caso, o código dentro do @media só será considerado caso a tela tenha no máximo 600px de largura.
```
	@media (orientation: landscape) {
		.caixa { 
			background-color: red;
		}
```	
Nesse outro caso só será aplicada a regra do @media quando o aparelho estiver no modo landscape.
Existem diversos tipos de parâmetros para colocarmos e garantirmos que o site seja totalmente responsivo.
		
#### Entendendo viewport

Podemos ter duas telas de mesmo tamanho mas com resoluções diferentes, ou seja, pixels diferentes. O mesmo acontece com aparelhos pequenos que podem ter resolução muito alta, seu tamanho de tela é pequeno mas sua resolução, pixels, é alta.
Viewport é a janela onde o site é exibido, é ele que define o funcionamento das media queries.
Nossa página precisa saber se está sendo acessada de um aparelho de tela pequena mas alta resolução, para isso nós manipulamos o viewport dentro do meta em nosso head.

Exemplo:
```
	<meta 
		name="viewport"
		content="width=device-width, initial-scale=1.0"
	>
```
#### Unidades de medidas flexíveis

Precisamos deixar os elementos responsivos ao tamanho do viewport, para isso utilizamos unidades de medida flexíveis.
Usamos o width em % e junto colocamos o max-width para manter o "tamanho" original da imagem.

Exemplo:
```
	.imagem {
		width: 100%
		max-width: 256px; <- largura original da imagem.
	}
```
#### Trabalhando com imagens

Para resolver o problema de carregamento de imagens no nosso site, precisamos que nossa página carregue imagens diferentes ao mesmo tempo.
Podemos ajudar o HTML a escolher automaticamente qual a melhor imagem que ele deve carregar utilizando o srcset.

Exemplo:
```
	<img srcset="imagens/gato-pequeno.jpg 200w,
				imagens/gato-grande.jpg 718w"
		sizes="(max-width: 200px) 200px, 400px"
		src="imagens/gato-grande.jpg"
		alt="foto de um gatinho" />
```

#### Outras técnicas de responsividade

* Pensar que nossas páginas poderão ser acessadas através de qualquer tipo de dispositivo
* Nunca deixar como algo essencial um funcionamento que possa sugerir que o usuário esteja acessando nosso site de um determinado dispositivo
* Pensar também em responsividade quando falamos sobre telas muito grandes
* Testar nosso site no máximo de dispositivos que conseguirmos antes de divulgá-lo


##### Links úteis: 

**ARTIGO** [Usando Media Queries no CSS](https://developer.mozilla.org/pt-BR/docs/Web/Guide/CSS/CSS_Media_queries)

**ARTIGO** [Trabalhando com viewport no CSS](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag)

**ARTIGO** [Trabalhando com imagens responsivas no CSS](https://developer.mozilla.org/pt-BR/docs/Aprender/HTML/Multimedia_and_embedding/Responsive_images)

## MÓDULO 13 - Boas Práticas com CSS

#### Padrões de nomenclatura - BEM

Uma das coisas mais difíceis na programação é dar nome às classes do html/css.
Para evitar problemas, escrevemos as classes dessa forma, com elementos e modificadores (que começam com --): 
	```
	--NO HTML: 
	<header class="topo">
		<a href="#" class="topo__link grande">Link do cabeçalho</a>
	</header>
	<footer class="rodape">
		<a href="#" class="rodape__link pequeno">Link do rodapé</a>
	</footer>
	```

	```
	/* NO CSS: */
	.topo {
		border: 1px solid green;
	}
	.topo__link {
		color: red;
	}
	.topo__link--grande {
		font-size: 20px;
	}
	
	.rodape {
		border: 1px solid blue;
	}
	.rodape__link {
		color: pink;
	}
	.rodape__link--pequeno {
		font-size: 8px;
	}
	```
Nesse caso, queremos que os links de rodapé e cabeçalho, que tem a mesma classe, tenham cores diferentes.

#### Tipos de arquitetura - SMACSS

SMACS - Scalable and Modular Architecture for CSS
Arquitetura escalável e Modular para CSS
Define uma estrutura de pastas para organizar nossos arquivos CSS

**Estrutura de Pastas:**

* Pasta base -> Seletores de elementos, pseudo-seletores e estilos globais. Ex: div, section, etc...
* Layout -> Elementos que são únicos na nossa página e, geralmente, representam as partes grandes do nosso site. Ex: header, main, footer, etc...
* Module -> Elementos que são reutilizados em diversos locais de nosso site. Ex: botões, listas, etc...
* State ->  Modificadores de nossos elementos. Ex: quando um botão está em foco, etc...
* Theme ->  Geralmente ficam as cores dos temas, tipos de fontes, etc... Usado apenas quando temos mais de uma opção de tema no nosso site. Ex: tema claro, tema escuro, etc...

#### Outras boas práticas com CSS

Utilizar metodologias de nomenclatura de classes e de estrutura de pastas ajuda quando trabalhamos em equipe
É sempre muito bom utilizar um guia de estilo (style guide) para padronizar a forma como escolhemos desenvolver nossos projetos
É importante sempre seguit os guias de estilos definidos nos projetos que iremos fazer parte


##### Links úteis:

**ARTIGO** [Entendendo o BEM no CSS](https://desenvolvimentoparaweb.com/css/bem/)

**ARTIGO** [Organize seu CSS com SMACSS, BEM e SASS](https://medium.com/@larymagal/organize-seu-css-com-smacss-bem-e-sass-7e8f50a41544)

**ARTIGO** [Entendendo Arquiteturas CSS](https://medium.com/tableless/arquitetura-css-d344fb01dd18)

## MÓDULO 14 - Principais ferramentas CSS

#### Frameworks

Ferramentas que disponibilizam funcionalidades pré-prontas
Diversos componentes já prontos
Classes que ajudam a montar layouts com rapidez

![Frameworks](https://cdn.hackr.io/uploads/posts/attachments/1679326591WjFOoim2eQ.png) "Exemplos de frameworks CSS.")

Exemplos: 
* Semantic UI
* TailwindCSS
* Foundation
* Bootstrap

**Dicas**
Sempre aprenda primeiro a fazer as coisas sem nenhum framework
Ao escolher utilizat um framework e qual iremos utilizar devemos analisar tecnicamente as nossas opções e escolher com base nessa análise

#### Pré-Processadores 

Cada um deles tem suas próprias regras para escrevermos o CSS
Funcionalidades a mais que dão mais poder ao nosso CSS
No final de tudo entrega um único CSS para o navegador poder exibir nossa página corretamente

Exemplos: 
* Sass
* Stylus


#### Teste de Qualidade de código - Lint

Ferramentas para avaliar se deixamos "escapar" algum código que não foi escrito seguindo o padrão que definimos (guia de estilos)
Também existem ferramentas parecidas para utilizarmos com pré-processadores CSS ou até mesmo com frameworks CSS
Ferramentas de lint são muito úteis para ajudar a garantir a qualidade dos nossos códigos

#### ResetCSS e NormalizeCSS

Adicionam um estilo base para o nosso projetos
Diminuem a chance de diferentes navegadores exibirem nosso site de diferentes maneiras
ResetCSS reseta a maioria dos estilos padrão dos elementos
NormalizeCSS normaliza os estilos padrão dos elementos para que eles tenham o mesmo estilo padrão em qualquer navegador

#### Styled-components

CSS-in-JS: CSS escrito dentro do Javascript
Utilizada geralmente junto com ReactJS e outros frameworks JavascriptAumenta muito mais as possibilidades de coisas que podemos fazer com o nosso CSS
Biblioteca: styled components

##### Links úteis:

**ARTIGO** [Semantic UI](https://semantic-ui.com/)

**ARTIGO** [Tailwind CSS](https://tailwindcss.com/)

**ARTIGO** [Foundation](https://get.foundation/)

**ARTIGO** [Bootstrap](https://getbootstrap.com.br/)

**ARTIGO** [SASS](https://sass-lang.com/)

**ARTIGO** [Stylus](https://stylus-lang.com/)

**ARTIGO** [CSS Lint](http://csslint.net/)

**ARTIGO** [Normalize CSS](https://necolas.github.io/normalize.css/)

**ARTIGO** [Reset CSS](https://meyerweb.com/eric/tools/css/reset/)

**ARTIGO** [Styled-components](https://styled-components.com/)

**ARTIGO** [Do Sass e BEM ao CSS-in-JS: A (re)evolução do CSS ao longo da história](https://www.felipefialho.com/blog/do-sass-e-bem-ao-css-in-js-a-evolucao-do-css-ao-longo-da-historia/)

## MÓDULO 15 - Projeto Final (Criando seu próprio site)

Será um site de portfólio, o meu se encontra no repositório abaixo:

[PORTFÓLIO LAURA PERRONI](#)
