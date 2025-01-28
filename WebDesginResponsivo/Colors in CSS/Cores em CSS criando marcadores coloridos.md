## Cores em CSS criando marcadores coloridos

O HTML da aula "Learn CSS Colors by Building a Set of Colored Markers" apresenta a estrutura de um conjunto de marcadores coloridos. Ele utiliza elementos básicos para criar um layout simples e prepara os estilos aplicados com CSS.

---

### *Estrutura HTML*
#### 1. *Cabeçalho do Documento (<head>):*
   - Define a codificação de caracteres e configurações para visualização responsiva.
   - Inclui o arquivo de estilos externo com <link rel="stylesheet" href="styles.css">.

#### 2. *Corpo do Documento (<body>):*
   - O título principal da página é definido com <h1> como "CSS Color Markers".
   - Um contêiner com a classe container agrupa os elementos visuais dos marcadores:
     - Cada marcador é representado por uma <div> com a classe marker e uma classe adicional que define sua cor (red, green ou blue).
     - Dentro de cada marcador, há duas subdivisões:
       - *<div class="cap">*: Representa a tampa do marcador.
       - *<div class="sleeve">*: Representa o corpo do marcador.

---

### *Características Aprendidas no HTML*
1. *Uso de classes múltiplas:* Combinações como marker red permitem reutilizar a classe marker para a estrutura geral e classes específicas para as cores.
2. *Agrupamento lógico:* A div principal (.container) organiza os marcadores para fácil estilização e alinhamento no CSS.
3. *Semântica simples:* Uso de elementos de divisão (<div>) para layout genérico.

---------------------------------



O CSS da aula “Learn CSS Colors by Building a Set of Colored Markers” complementa o HTML ao aplicar estilos que criam os marcadores coloridos. Ele utiliza propriedades de layout e manipulação de cores para destacar os elementos visuais. Abaixo está o resumo do que foi ensinado:

---

### *Resumo do CSS*
#### 1. *Estilização Geral:*
   - *Título (<h1>):*
     - O título é centralizado usando text-align: center.

   - *Contêiner (.container):*
     - Fundo branco definido com background-color: rgb(255, 255, 255).
     - Adicionado espaçamento vertical interno com padding: 10px 0.

---

#### 2. *Estrutura dos Marcadores:*
   - *marker:*
     - Define a largura dos marcadores como 200px e a altura como 25px.
     - Margens automáticas (margin: 10px auto) centralizam os marcadores horizontalmente e criam espaçamento vertical.
   - *cap e sleeve:*
     - Ambos são configurados como elementos em linha (display: inline-block) para ficarem lado a lado.
     - *Cap:*
       - Largura de 60px e altura de 25px.
     - *Sleeve:*
       - Largura de 110px e altura de 25px.
       - Fundo semitransparente configurado com rgba(255, 255, 255, 0.5).
       - Borda à esquerda estilizada com border-left: 10px double rgba(0, 0, 0, 0.75).

---

#### 3. *Cores dos Marcadores:*
Cada marcador (.red, .green, .blue) utiliza *gradientes lineares* e *sombreamento (box-shadow)* para criar efeitos realistas.

   - *Vermelho (.red):*
     - Gradiente linear com tons em *RGB*:
       - Começa com um marrom avermelhado rgb(122, 74, 14).
       - Vai para um rosa forte rgb(245, 62, 113).
       - Termina com vermelho profundo rgb(162, 27, 27).
     - Adicionado efeito de brilho vermelho escuro com box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8).

   - *Verde (.green):*
     - Gradiente linear com tons em *hexadecimal*:
       - Começa com verde oliva escuro #55680D.
       - Vai para verde brilhante #71F53E.
       - Termina com verde intenso #116C31.
     - Sombra verde configurada com box-shadow: 0 0 20px 0 #3B7E20CC.

   - *Azul (.blue):*
     - Gradiente linear com tons em *HSL*:
       - Começa com azul petróleo hsl(186, 76%, 16%).
       - Vai para azul claro hsl(223, 90%, 60%).
       - Termina com azul escuro hsl(240, 56%, 42%).
     - Sombra azul adicionada com box-shadow: 0 0 20px 0 blue.

---

### *Conceitos Reforçados no CSS*
1. *Cores:*
   - Aprendizado das diferentes notações de cores:
     - *RGB*: Mistura de vermelho, verde e azul.
     - *Hexadecimal*: Representação compacta de cores.
     - *HSL*: Define cor por tonalidade, saturação e luminosidade.
   - Utilização de transparência com *RGBA*.

2. *Gradientes Lineares:*
   - Uso de linear-gradient() para criar transições suaves entre várias cores.

3. *Sombras:*
   - box-shadow para criar efeitos de luz e profundidade.

4. *Layout:*
   - Centralização com margin: auto.
   - Alinhamento lado a lado usando display: inline-block.

---

### *Resultado Final*
Esse CSS transforma simples `<div>`s em representações visuais realistas de marcadores coloridos com efeitos de gradiente, sombras e estrutura bem definida.