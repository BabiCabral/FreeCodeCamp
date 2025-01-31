

## *Learn Forms by Building a Registration Form*  

Essa aula ensinou conceitos fundamentais sobre *formulários em HTML* e sua estilização com *CSS*. O foco foi na organização dos campos de entrada e na aplicação de estilos para melhorar a aparência do formulário.  

---

##  *Revisão do Código HTML*
O formulário está bem estruturado com diferentes tipos de campos de entrada:

### *1. Estrutura e Agrupamento (<fieldset> e <label>)*
- O uso de <fieldset> ajuda a *organizar os campos* e cria separação visual no formulário.  
- *Rótulos (<label>)* são usados para associar cada campo ao seu propósito, melhorando a acessibilidade.

### *2. Inputs e Validação*
- *Text inputs* (type="text", type="email", type="password") permitem a inserção de dados.  
- *Restrições de validação*:  
  - O campo de senha (type="password") exige *pelo menos 8 caracteres* formados por letras minúsculas e números de 0 a 5 (pattern="[a-z0-5]{8,}").  
  - O campo de idade (type="number") só aceita valores entre *13 e 120 anos* (min="13" max="120").  
  - O checkbox dos termos de uso (required) precisa ser marcado para permitir o envio do formulário.  

### *3. Seleção de Opções*
- *Botões de rádio (<input type="radio">)*: o usuário pode escolher entre "Personal" ou "Business".  
- *Seleção (<select>)*: dropdown para o usuário escolher como descobriu o site.  

### *4. Envio do Formulário*
- O botão de envio (<input type="submit" value="Submit">) permite enviar os dados.

---

## *Revisão do Código CSS*
O CSS aplicado melhora a *legibilidade, usabilidade e aparência geral* do formulário.

### *1. Estilização Geral*
- O fundo da página tem um *tom escuro* (background-color: #1b1b32;) e o texto é branco (color: #f5f6f7;) para contraste.  
- Fonte utilizada: *Tahoma*.  
- O formulário tem *largura responsiva* (width: 60vw; max-width: 500px; min-width: 300px;).  

### *2. Campos de Entrada (input, textarea, select)*
- Os campos são largos (width: 100%) e têm altura mínima (min-height: 2em) para facilitar a digitação.  
- Campos de texto têm *fundo escuro* (background-color: #0a0a23;) e texto branco.  

### *3. Separação Visual*
- *<fieldset>* tem uma linha de separação inferior (border-bottom: 3px solid #3b3b4f;).  
- O último <fieldset> não tem borda para um visual mais limpo (fieldset:last-of-type { border-bottom: none; }).  

### *4. Botão de Envio*
- O botão de envio (input[type="submit"]) tem um *tamanho adequado* e um fundo escuro para manter a harmonia com o design.  
- Ele ocupa *60% da largura total, mas nunca menos de **300px* para garantir usabilidade.  

---

## *Conclusão*
Essa aula mostrou como *estruturar formulários corretamente e aplicar estilos para melhorar a experiência do usuário*. O que foi aprendido:  
✅ Como agrupar campos com <fieldset> para organização.  
✅ Como aplicar *validações HTML* (required, pattern, min, max).  
✅ Como estilizar formulários para melhor *acessibilidade e usabilidade*.  

