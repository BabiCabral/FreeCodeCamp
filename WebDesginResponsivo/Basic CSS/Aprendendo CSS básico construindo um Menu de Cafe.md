## Aprendendo CSS básico construindo um Menu de Café

### Estrutura HTML*

#### 1. *Cabeçalho do documento (<head>):*
   - Define a codificação de caracteres como UTF-8.
   - Inclui o arquivo CSS externo através de <link rel="stylesheet" href="styles.css">.

#### 2. *Corpo do documento (<body>):*
   - O menu está organizado em uma <div> com a classe menu, o que permite aplicar estilos consistentes ao layout.
   - Contém as seguintes seções principais:
     - *<main>:* Abriga o conteúdo principal da página, incluindo:
       - *Título e subtítulo do café:* O <h1> contém o nome do café, e <p> com a classe established exibe a data de fundação.
       - *Divisão do menu em categorias:*
         - Cada categoria (como "Coffee" e "Desserts") está dentro de uma <section>.
         - Um ícone representativo é inserido com <img> para melhorar a experiência visual.
         - Os itens de cada categoria são representados por <article>:
           - *Nome do item:* Utiliza a classe flavor ou dessert.
           - *Preço:* Exibido com a classe price.
     - *Linha divisória:* Um <hr> separa visualmente os elementos.
   - *Rodapé (<footer>):*
     - Contém um link para o site oficial (<a> com atributo target="_blank" para abrir em uma nova aba).
     - Um parágrafo com a classe address exibe o endereço fictício.

---

### *Boas práticas e conceitos destacados no HTML*
1. *Estrutura semântica:* Uso correto de tags como <main>, <section>, <article> e <footer> para criar um documento acessível e bem estruturado.

2. *Classes CSS:* Cada elemento possui classes específicas (menu, established, flavor, price, etc.) para estilização no CSS.

3. *Imagens com atributos alt:* Melhora a acessibilidade, permitindo que leitores de tela descrevam as imagens.

4. *Links externos:* Atributo target="_blank" usado para abrir links em novas abas.

   -----------------------------------

   ​

### Resumo do CSS*

#### 1. *Estilização Geral:*
   - *Background do corpo (body):*
     - Uma imagem de fundo de grãos de café é definida com background-image.
     - A fonte padrão do texto é configurada para sans-serif.
     - Um espaçamento geral de 20px é adicionado ao redor da página com padding.
   - *Fonte e Alinhamento:*
     - Títulos (h1 e h2) utilizam a fonte Impact com uma opção de fallback serif.
     - Os textos dos títulos, parágrafos e subtítulos são centralizados com text-align: center.

---

#### 2. *Estilização do Container do Menu:*
   - A classe .menu:
     - Define um fundo com cor *burlywood* para destacar o menu.
     - Define largura responsiva de *80%* do tamanho da tela, com um limite máximo de *500px*.
     - Aplica margens automáticas para centralizar o menu horizontalmente.
     - Adiciona espaçamento interno com padding: 20px.

---

#### 3. *Linhas Divisórias (<hr>):*
   - Personalização das linhas:
     - Altura definida como 2px.
     - Cor de fundo e borda definidas como *marrom* (brown).

---

#### 4. *Estilização de Imagens:*
   - As imagens são centralizadas usando:
     css
     display: block;
     margin-left: auto;
     margin-right: auto;


---

#### 5. *Itens do Menu (.item):*
   - *Organização interna:* 
     - As descrições (flavor, dessert) e os preços (price) usam display: inline-block para ficarem lado a lado.
     - Larguras proporcionais:
       - flavor e dessert ocupam 75% da linha.
       - price ocupa os outros 25%.
     - Textos alinhados:
       - Os nomes dos itens ficam à esquerda com text-align: left.
       - Os preços são alinhados à direita com text-align: right.

---

#### 6. *Estilização do Rodapé (footer):*
   - Fonte reduzida com font-size: 14px.
   - Margem inferior ajustada na classe .address para criar espaçamento.

---

#### 7. *Links no Rodapé:*
   - Cores dos links (<a>):
     - Cor inicial: black.
     - Quando visitado (a:visited): mantém a cor black.
     - Quando o cursor passa por cima (a:hover): cor muda para *marrom* (brown).
     - Quando o link é ativado/clicado (a:active): também fica marrom.

---

### *Conceitos Reforçados no CSS*
1. *Classes para Modularidade:*
   - Uso de classes como .menu, .item, .flavor e .price para segmentar o design.
2. *Estilo Responsivo:*
   - width: 80% com max-width: 500px no menu garante que ele funcione bem em dispositivos de diferentes tamanhos.
3. *Controle de Layout com Inline-Block:*
   - display: inline-block organiza os itens de forma elegante em uma mesma linha (descrição e preço).
4. *Pseudoclasses de Links:*
   - Uso de :hover, :visited e :active para criar interatividade nos links.
5. *Hierarquia de Fontes:*
   - Fontes distintas para títulos e corpo criam contraste visual.