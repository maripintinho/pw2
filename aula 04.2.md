##### **Display: block, inline e inline-block**

No HTML e no CSS, os elementos podem se comportar basicamente de três formas:

* **Elementos de bloco (block)**
* **Elementos em linha (inline)**
* **Elementos em linha-bloco (inline-block)**



Esse comportamento influencia como eles ocupam esse espaço na página e como se organizam no layout.



**De forma geral:**

* **Block** organiza a página
* **Inline** organiza o texto -> não usa width e height
* **Inline-block** organiza componentes visuais



###### **Elementos de Bloco (display: block)**

*Como funcionam:*

* Sempre começam em uma nova linha
* Ocupam toda a largura disponível do elemento pai
* Aceitam normalmente:

&#x20;  - width e height

&#x20;  - margin (top, right, bottom e left)

&#x20;  -padding

* Empurram outros elementos para baixo

Exemplos comuns:

<div>, <p>, <h1> a <h6>, <section>, <article>, <header>, <footer>

\-> organizam a página



###### **Elementos em Linha (display: inline)**

*Como funcionam:*

* Não quebram linha
* Ocupam apenas o espaço do conteúdo
* Fluem com o texto
* Não aceitam:

&#x20;  - width e height

&#x20;  - margin e padding

&#x20;  - (funcionam apenas horizontalmente\_

* Usados principalmente dentro de textos

Exemplos comuns:

<span>, <a>, <strong>, <em>, <label>

\-> organizam o texto



###### **Elementos Bloco em Linha (display: inline-block)**

*Como funcionam:*

* Ficam na mesma linha (como inline)
* Mas aceitam:

&#x20;  - width e height

&#x20;  - margin e padding (como block)

* Não forçam quebra de linha
* Muito usados para criar cards, botões e menus horizontais.

Exemplos comuns:

<img>, <button>, <input>

\->organizam componentes visuais



###### **Flexbox: O Poder dos Layouts Unidimensionais**

Flexbox é um modelo de layout unidimensional que distribui espaço e alinha itens em uma linha ou coluna.

Revolucionou a forma como criamos layouts responsivos, eliminando hacks com *float e position*.

Se aplica:

**display: flex** ou **display: inline-flex**



Quando **Flex-Direction** for\*\*: row ,\*\* então:

align-items: posiciona verticalmente com start-center-end-strech

justify-content: posiciona horizontalmente com start-center-end



Quando **Flex-Direction** for\*\*: column\*\* , então:

align-items: posiciona horizontalmente com start-center-end-strech

justify-content: posiciona verticalmente com start-center-end



&#x20;

