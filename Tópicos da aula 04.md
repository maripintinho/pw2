Tópicos da aula 04

\- esquemas de posicionamento (static, relative, absolute, fixed e sticky)

\- display

\- layout flexbox



Esquemas de posicionamento

**Static (Padrão)**: O posicionamento estático é o comportamento natural. Propriedades **top, right, bottom, left** não têm, efeito.

*.elemento* {

&#x20; position: static;

&#x20; */\*Comportamento padrão\*/*

}





**Relative**: O elemento mantém seu espaço original no fluxo, mas pode ser deslocado visualmente usando **top, right, bottom, left**. Outros elementos não são afetados.

.*elemento* {

&#x20; position: relative;

&#x20; top: 20px;

&#x20; left: 30px;

}



**Absolute**: Remove o elemento do fluxo normal. Pode ser deslocado visualmente usando **top, right, bottom, left.** Usado nos sites como mensagens, janelas, propagandas, pois é como uma camada a parte da página.

*.modal* {

&#x20; position: absolute;

&#x20; top: 50%;

&#x20; left: 50%;

&#x20; transform: translate(-50%, -50%);

}

Se houver mais de um absolute, utiliza-se a propriedade **z-index** -> controla a ordem de empilhamento. Só funciona em elementos que possuem uma posição definida (relative, absolute, fixed, sticky). **O *z-indez* controla o eixo z da página.** Valor se dá quanto maior o número, mais à frente; quanto menor o número, mais ao fundo

.*elemento1* {

&#x20; position: absolute;

&#x20; z-indez: 1;

}





**Fixed**: Posiciona o elemento em relação à janela do navegador (viewport). Permanece fixo mesmo com rolagem da página.

*.header* {

&#x20; position: fixed;

&#x20; top: 0;

&#x20; left: 0;

&#x20; width: 100;

&#x20; z-index: 1000;

}



**Sticky**: O elemento se comporta como **relative** até que atinja um limite definido durante a rolagem, quando "**gruda**" como fixed. Tipo cabeçalhos de tabelas.

**Requisitos Importantes**

* Definir ao menos uma direção (top, bottom, left, right)
* O elemento pai deve ter altura suficiente
* Não funciona com overflow: hidden no pai

*.sidebar-nav* {

position: sticky;

top: 20px;

/\*Gruda quando chega a 20px do topo \*/

}

