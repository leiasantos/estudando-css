<h1>CSS - Guia para Estilos em Páginas Web</h1>
<p>"Cascading Style Sheets" (Folhas de Estilo em Cascata, em português)
</p>

<h2>💬 Comentários em CSS</h2>
<p>* Comentários em CSS Usa se o /*  */ </p>
<pre>
  <code>/* Este é um comentário */
h1 {
  color: blue;
}
</code>
</pre>

<h2>Anatomia</h2>
<p>A "anatomia" do CSS refere-se à estrutura básica de uma regra CSS, que define como os elementos de uma página web devem ser estilizados. 
</p>
<ol>
  <li> Seletores</li>
  <li> Propriedades</li>
  <li>Valores</li>
  <li>Declaração</li>
  <li>Bloco de Declaração</li>
  <li>Regra CSS</li>
</ol>
<pre>
  <code>
    h1{
    color: blue;
    font-size:60px
    text-transform: uppercase;
}</code>
</pre>

<h2> Características do Cascading</h2>
<ol>
  <li>Hierarquia de Especificidade</li>
  <li>Importância</li>
  <li>Origem do Estilo</li>
  <li>Ordem das Regras</li>
  <li>Herdabilidade (Inheritance)</li>
  <li>Valores Padrão e Herança</li>
</ol>
<h2>Cada seletor tem um peso, soma dos pesos faz as declarações serem aplicadas.</h2>
<ol>
  <li>#id - 100</li>
  <li>.class - 10</li>
  <li>element - 1</li>
</ol>

<h2> Valores e unidades de medidas</h2>
<p>Cada propriedade possui valores 
'property: value'</p>

<ol>
  <li>Valores Numéricos</li>
  <li>Unidades de Medida Absolutas</li>
  <li>Unidades de Medida Relativas</li>
</ol>

<h2>Valores absolutos</h2>
<table>
        <thead>
            <tr>
                <th>Unidade</th>
                <th>Descrição</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>cm</td>
                <td>Centímetro</td>
            </tr>
            <tr>
                <td>mm</td>
                <td>Milímetros</td>
            </tr>
            <tr>
                <td>in</td>
                <td>Polegadas</td>
            </tr>
            <tr>
                <td>px</td>
                <td>Pixels</td>
            </tr>
            <tr>
                <td>pt</td>
                <td>Pontos</td>
            </tr>
            <tr>
                <td>pc</td>
                <td>Paica</td>
            </tr>
        </tbody>
    </table>

 <h2>Unidades de Medida Relativas</h2>
<table>
        <thead>
            <tr>
                <th>Unidade</th>
                <th>Descrição</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>em</td>
                <td>1 em é uma vez o <code>font-size</code> do elemento.</td>
            </tr>
            <tr>
                <td>rem</td>
                <td>1 rem é uma vez o <code>font-size</code> do elemento acima na hierarquia de elementos.</td>
            </tr>
            <tr>
                <td>vw</td>
                <td>1vw é 1% da largura da janela do navegador.</td>
            </tr>
            <tr>
                <td>vh</td>
                <td>1vh é 1% da altura da janela do navegador.</td>
            </tr>
            <tr>
                <td>vmin</td>
                <td>1vmin é 1% da menor dimensão da janela do navegador.</td>
            </tr>
            <tr>
                <td>vmax</td>
                <td>1vmax é 1% da maior dimensão da janela do navegador.</td>
            </tr>
            <tr>
                <td>%</td>
                <td>Calcula o tamanho relativo ao elemento pai.</td>
            </tr>
        </tbody>
    </table>

<h2>Seletores</h2>
<ul>
  <li>id</li>
  <li>class</li>
  <li>type| element| tag</li>
  <li>atributo</li>
  <li>universal</li>
</ul>

<h2> Combinator em css</h2>
<p>Combinadores no CSS são usados para combinar seletores de maneiras diferentes, 
  permitindo que você selecione elementos com base em sua relação com outros elementos.
  Existem quatro principais tipos de combinadores no CSS: descendente, filho, irmão adjacente, e irmão geral.
</p>

<ul>
  <li>Descendent</li>
  <li>List</li>
  <li>Next sibling</li>
  <li>Child</li>
</ul>

<h2> Box model</h2>
<p>Tudo são caixas
Todos os elementos HTML serão considerados uma caixa, assim como uma caixa de papelão.
</p>
<p>Caixas possuem determinadas propriedades:</p>
<ul>
  <li>Conteúdo</li>
  <li>Largura</li>
  <li>Preenchimento (espaço interno)</li>
  <li>Espaçamento (espaço externo)</li>
</ul>

<h2> Display</h2>
<p>A propriedade display no CSS é uma das mais importantes para controlar o layout dos elementos na página.
  Ela determina como os elementos são exibidos na página e como eles interagem com outros elementos.</p>
<ul>
  <li>block</li>
  <li>inline</li>
  <li>inline-block</li>
  <li>flex</li>
  <li>grid</li>
  <li>none</li>
  <li>list-item</li>
</ul>
<table>
        <thead>
            <tr>
                <th>Valor</th>
                <th>Descrição</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>display: block</td>
                <td>É um elemento de bloco. Ele ocupa toda a largura disponível e inicia uma nova linha.</td>
            </tr>
            <tr>
                <td>display: inline</td>
                <td>O elemento é exibido na mesma linha que outros elementos em linha. O elemento só ocupa o espaço necessário para o seu conteúdo e não inicia uma nova linha.</td>
            </tr>
            <tr>
                <td>display: inline-block</td>
                <td>Combina características de elementos de bloco e em linha. O elemento é exibido em linha, mas permite definir largura e altura.</td>
            </tr>
            <tr>
                <td>display: flex</td>
                <td>O elemento se torna um contêiner flexível, permitindo a disposição de seus itens filhos usando o Flexbox.</td>
            </tr>
            <tr>
                <td>display: grid</td>
                <td>O elemento se torna um contêiner de grid, permitindo o uso do CSS Grid Layout para criar layouts em grade.</td>
            </tr>
            <tr>
                <td>display: none</td>
                <td>O elemento não é exibido na página e não ocupa espaço. É como se ele fosse removido do layout.</td>
            </tr>
            <tr>
                <td>display: list-item</td>
                <td>O elemento é exibido como um item de lista, com um marcador (ou outro marcador de lista).</td>
            </tr>
        </tbody>
    </table>

<h2>Border</h2>
<p>Esse elemento define a borda de um elemento.</p>
<p>Estilos de bordas:</p>

<ul>
  <li>dotted</li>
  <li>dashed</li>
  <li>solid </li>
  <li> double</li>
    <li>groove </li>
  <li>ridge</li>
    <li> outset</li>
</ul>


<h2>Width e Height</h2>
<p>Width </p>
<ul>
  <li>width: define a largura do elemento </li>
  <li>min-width: largura mínima</li>
  <li>max-width: largura máxima</li>
  <li></li>
</ul>

<p>Height</p>
<ul>
  <li>height: define a altura do elemento </li>
  <li>min-height: altura mínima</li>
  <li>max-height: altura máxima</li>
</ul>

<h2>Margin</h2>
<p>É usada para criar espaço ao redor de elementos, fora das bordas. Ela
pode ser usada para adicionar espaçamento entre elementos ou para
centralizar elementos dentro de um contêiner.</p>

<ul>
  <li>margin-top: define o espaço acima do elemento.</li>
  <li>margin-right: define o espaço à direita do elemento.</li>
  <li> margin-bottom: define o espaço abaixo do elemento.</li>
  <li>margin-left: define o espaço à esquerda do elemento.</li>
</ul>

<h2>Padding</h2>
<p>É  usada para criar espaço interno ao redor do conteúdo de um elemento, dentro das suas bordas. Ele controla o espaçamento entre o conteúdo do elemento e suas bordas, afetando diretamente o tamanho do elemento sem alterar suas margens.</p>

<ul>
  <li>padding-top: indica qual o espaçamento superior no elemento.</li>
  <li>padding-right: indica a distância aplicada no lado direito do elemento;</li>
  <li>padding-bottom: indica a distância na parte inferior do conteúdo;</li>
  <li>padding-left:  representa a distância no lado esquerdo do box;
</li>
</ul>

<h2> Fontes e textos</h2>
 <table>
        <thead>
            <tr>
                <th>Propriedade</th>
                <th>Descrição</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>font-family</td>
                <td>Define a família de fontes a ser usada no texto.</td>
            </tr>
            <tr>
                <td>font-size</td>
                <td>Define o tamanho da fonte.</td>
            </tr>
            <tr>
                <td>font-weight</td>
                <td>Define a espessura da fonte.</td>
            </tr>
            <tr>
                <td>line-height</td>
                <td>Define a altura da linha, que é o espaço entre linhas de texto.</td>
            </tr>
            <tr>
                <td>font-variant</td>
                <td>Define variações estilísticas como <code>small-caps</code>.</td>
            </tr>
            <tr>
                <td>letter-spacing</td>
                <td>Define o espaçamento entre caracteres.</td>
            </tr>
            <tr>
                <td>text-align</td>
                <td>Alinha o texto dentro de seu contêiner.</td>
            </tr>
            <tr>
                <td>color</td>
                <td>Define a cor do texto.</td>
            </tr>
            <tr>
                <td>text-decoration</td>
                <td>Adiciona ou remove decorações de texto (como <code>underline</code>).</td>
            </tr>
            <tr>
                <td>text-shadow</td>
                <td>Adiciona uma sombra ao texto.</td>
            </tr>
            <tr>
                <td>word-spacing</td>
                <td>Define o espaçamento entre palavras.</td>
            </tr>
            <tr>
                <td>white-space</td>
                <td>Controla como o espaço em branco dentro de um elemento é tratado.</td>
            </tr>
            <tr>
                <td>text-indent</td>
                <td>Indenta a primeira linha de um parágrafo.</td>
            </tr>
            <tr>
                <td>text-transform</td>
                <td>Controla a capitalização do texto (como <code>uppercase</code> ou <code>capitalize</code>).</td>
            </tr>
        </tbody>
    </table>

<h2>background</h2>
 <table>
        <thead>
            <tr>
                <th>Propriedade</th>
                <th>Descrição</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>background-color</td>
                <td>Define a cor de fundo de um elemento.</td>
            </tr>
            <tr>
                <td>background-image</td>
                <td>Define uma imagem de fundo para um elemento.</td>
            </tr>
            <tr>
                <td>background-repeat</td>
                <td>Controla se e como a imagem de fundo se repete.</td>
            </tr>
            <tr>
                <td>background-position</td>
                <td>Define a posição inicial da imagem de fundo dentro do elemento.</td>
            </tr>
            <tr>
                <td>background-size</td>
                <td>Controla o tamanho da imagem de fundo.</td>
            </tr>
        </tbody>
    </table>

<h2>Position</h2>
  <table>
        <thead>
            <tr>
                <th>Valor</th>
                <th>Descrição</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>static</td>
                <td>Este é o valor padrão. O elemento é posicionado conforme o fluxo normal da página, sem possibilidade de ajuste adicional com as propriedades top, right, bottom e left.</td>
            </tr>
            <tr>
                <td>relative</td>
                <td>O elemento é posicionado em relação à sua posição original no fluxo da página. Você pode ajustar sua posição usando top, right, bottom e left, mas o espaço original do elemento ainda será mantido.</td>
            </tr>
            <tr>
                <td>absolute</td>
                <td>O elemento é removido do fluxo normal da página e posicionado em relação ao seu elemento ancestral mais próximo que tenha uma posição diferente de static (geralmente o primeiro ancestral com relative, absolute, fixed ou sticky). Caso não haja um ancestral posicionado, ele será posicionado em relação ao viewport.</td>
            </tr>
            <tr>
                <td>fixed</td>
                <td>O elemento é removido do fluxo normal da página e é posicionado em relação ao viewport, permanecendo fixo na tela mesmo quando a página é rolada.</td>
            </tr>
            <tr>
                <td>sticky</td>
                <td>O elemento é posicionado conforme o fluxo normal da página até que um determinado ponto de rolagem seja alcançado. A partir desse ponto, ele se comporta como fixed, ficando preso à posição especificada em relação ao viewport.</td>
            </tr>
        </tbody>
    </table>

<h2>Seletores</h2>
<h3>Pseudo-Classes</h3>
<p>As pseudo-classes permitem selecionar elementos com base em seu estado ou posição no documento, sem a necessidade de adicionar classes ou IDs diretamente aos elementos.</p>
<ul>
  <li>:hover
Seleciona um elemento quando o mouse passa sobre ele. Comumente usado para criar efeitos visuais interativos, como mudanças de cor ou estilo de botão.</li>
<pre>
  <code>
  a:hover {
  color: red;
}
  </code>
</pre>
  <li>:nth-child(): Seleciona elementos baseados em uma posição específica dentro de seu pai.</li>
  <li>:not(): Seleciona todos os elementos que não correspondem a um seletor específico.</li>
  <pre>
  <code>
  li:nth-child(odd) {
  background-color: lightgray;
}
  </code>
</pre>
  <li>:first-child: Seleciona o primeiro filho de um elemento.</li>
   <li>:last-child: Seleciona o último filho de um elemento</li>
  <pre>
  <code>
  p:first-child {
  font-weight: bold;
}</code>
</pre>
</ul>

<h2>Pseudo-Elements</h2>
<p>Os pseudo-elementos permitem estilizar partes específicas de um elemento, como o início ou o fim do conteúdo, ou até mesmo inserir conteúdo sem modificar o HTML.</p>
<ul>
  <li>:first-letter
Aplica estilo à primeira letra de um elemento. Usado para efeitos tipográficos, como na formatação de parágrafos ou artigos.</li>
  <pre>
  <code>
  p:first-letter {
  font-size: 2em;
  color: blue;
}
</code>
</pre>
  <li>:before
Insere conteúdo antes do conteúdo real do elemento. É frequentemente usado para adicionar ícones ou outros elementos decorativos.</li>
  <pre>
  <code>div::before {
  content: "🔹";
  margin-right: 10px;
}
</code>
</pre>
  <li>:after
Insere conteúdo após o conteúdo real do elemento. Semelhante ao :before, mas coloca o conteúdo no final do elemento.</li>
  <pre>
  <code>
  div::after {
  content: "✔️";
  margin-left: 10px;
}
</code>
</pre>
 


