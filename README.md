**Atividade de Pesquisa: Introdução ao JavaScript**
Objetivo:
Introduzir os alunos ao JavaScript, explorando suas principais características e aplicando conceitos básicos em pequenos projetos práticos.

![](javas.png)

### 1) **O que é JavaScript?**

### - **Defina JavaScript e sua principal função no desenvolvimento web:**

JavaScript é uma linguagem de programação interpretada, de alto nível e multiparadigma, amplamente utilizada no desenvolvimento web. É uma das três principais tecnologias da web, junto com HTML e CSS. A principal função de JavaScript no desenvolvimento web é tornar as páginas interativas e dinâmicas. Enquanto o HTML é responsável por estruturar o conteúdo e o CSS por estilizar as páginas, o JavaScript adiciona comportamento e funcionalidades. 

Com JavaScript, é possível manipular o DOM (Document Object Model) para atualizar elementos HTML dinamicamente, permitindo que o conteúdo de uma página seja alterado em resposta a interações do usuário, como cliques e movimentos do mouse. Também é usado para validar formulários, garantindo que os dados inseridos pelo usuário estejam corretos antes do envio. Além disso, JavaScript permite realizar comunicação assíncrona com servidores por meio de AJAX, possibilitando a atualização de partes da página sem a necessidade de recarregá-la completamente.

Outra importante aplicação de JavaScript é na criação de animações e efeitos visuais que melhoram a experiência do usuário, como menus deslizantes e transições suaves.

### - **Pesquise sobre a história do JavaScript e sua evolução ao longo dos anos:**

Foi criado em 1995 por Brendan Eich enquanto trabalhava na Netscape Communications. Originalmente chamado de Mocha, depois renomeado para LiveScript, e finalmente para JavaScript, o nome reflete a colaboração da Netscape com a Sun Microsystems, criadora da linguagem Java. JavaScript foi introduzido no navegador Netscape Navigator 2.0, permitindo páginas web mais interativas em comparação com a natureza estática do HTML.

Em 1997, JavaScript foi padronizado como ECMAScript (ES) pela ECMA International, com a primeira versão, ES1, lançada nesse ano. Essa padronização foi crucial para garantir consistência entre diferentes navegadores web, permitindo que os desenvolvedores escrevessem código que funcionasse de forma confiável em várias plataformas.

Ao longo dos anos, JavaScript evoluiu significativamente:

- **ES3 (1999)**: Introduziu expressões regulares, tratamento de exceções com try-catch, entre outras funcionalidades.
- **ES5 (2009)**: Adicionou "strict mode", suporte a JSON, e métodos adicionais para arrays e objetos.
- **ES6 (2015)**: Uma grande atualização que introduziu classes, promessas, funções de seta (arrow functions), literais de template, e declarações de variáveis com `let` e `const`. As versões pós-ES6 passaram a ser nomeadas pelo ano de lançamento (por exemplo, ES2016, ES2017).
- **Atualizações Recentes**: Atualizações anuais adicionaram recursos como `async/await`, novos métodos de array, o objeto `globalThis`, e mais.

JavaScript também se expandiu além do navegador. O Node.js, introduzido em 2009, permitiu o uso de JavaScript para o desenvolvimento do lado do servidor, ampliando ainda mais seu escopo de aplicação. A versatilidade do JavaScript agora se estende a aplicativos desktop e móveis, tornando-o um pilar fundamental do desenvolvimento web moderno.

Ao longo de sua evolução, o padrão ECMAScript tem sido mantido pelo TC39, um grupo de desenvolvedores, organizações e empresas comprometidas com o avanço da linguagem. Esse desenvolvimento contínuo manteve o JavaScript na vanguarda das tecnologias web, garantindo que continue relevante e poderoso para aplicações modernas.

### 2) **Características Básicas do JavaScript:**

### - **O que são variáveis e como são declaradas em JavaScript?**

Em JavaScript, variáveis são usadas para armazenar e manipular dados. Você pode pensar em variáveis como "caixas" que contêm informações. Existem três formas principais de declarar variáveis em JavaScript:

1. **`var`**: A declaração `var` é a forma mais antiga de declarar variáveis. As variáveis declaradas com `var` são funcionais, o que significa que são acessíveis em todo o bloco de código onde foram declaradas (ou em toda a função se estiver dentro de uma função). No entanto, `var` tem alguns problemas, como o "hoisting" (elevação), onde a variável é movida para o topo do seu contexto de execução.

   ```javascript
   var nome = 'João';
   ```

2. **`let`**: A declaração `let` foi introduzida no ECMAScript 6 (ES6) e é usada para criar variáveis com escopo de bloco. Isso significa que a variável é acessível apenas dentro do bloco onde foi declarada. `let` também resolve alguns problemas relacionados ao `var`, como o hoisting.

   ```javascript
   let idade = 30;
   ```

3. **`const`**: A declaração `const` também foi introduzida no ES6 e é usada para criar variáveis que não podem ser reatribuídas depois de inicializadas. Como `let`, `const` tem escopo de bloco. No entanto, isso não significa que o valor armazenado na variável é imutável; se o valor for um objeto ou array, suas propriedades ainda podem ser alteradas.

   ```javascript
   const pi = 3.14159;
   ```

Para declarar uma variável em JavaScript, você escolhe uma dessas palavras-chave (`var`, `let` ou `const`), seguida pelo nome da variável e, opcionalmente, inicializa com um valor. Por exemplo:

```javascript
let nome = 'Ana';
const idade = 25;
```


### - **Quais são os principais tipos de dados em JavaScript? (Exemplo: número, string, booleano, array, objeto):**

JavaScript possui vários tipos de dados principais que podem ser utilizados para armazenar diferentes tipos de informações. Aqui estão os principais tipos de dados em JavaScript, junto com exemplos:

1. **Número (Number)**: Representa tanto números inteiros quanto de ponto flutuante.
   ```javascript
   let inteiro = 42;
   let decimal = 3.14;
   ```

2. **String**: Representa uma sequência de caracteres. Pode ser delimitada por aspas simples (`'`), aspas duplas (`"`), ou crases (\`).
   ```javascript
   let texto1 = 'Olá, mundo!';
   let texto2 = "JavaScript é divertido!";
   let texto3 = `Interpolação: ${texto1}`;
   ```

3. **Booleano (Boolean)**: Representa um valor lógico que pode ser verdadeiro (`true`) ou falso (`false`).
   ```javascript
   let verdade = true;
   let falso = false;
   ```

4. **Array**: Um objeto especial para armazenar listas ordenadas de valores.
   ```javascript
   let frutas = ['maçã', 'banana', 'laranja'];
   let numeros = [1, 2, 3, 4, 5];
   ```

5. **Objeto (Object)**: Uma coleção de propriedades, onde cada propriedade é uma associação entre uma chave (nome) e um valor.
   ```javascript
   let pessoa = {
       nome: 'Carlos',
       idade: 30,
       profissao: 'Desenvolvedor'
   };
   ```

6. **Nulo (Null)**: Representa a ausência intencional de qualquer valor.
   ```javascript
   let valorNulo = null;
   ```

7. **Indefinido (Undefined)**: Uma variável que foi declarada mas ainda não foi atribuída com um valor.
   ```javascript
   let valorIndefinido;
   ```

8. **Símbolo (Symbol)**: Um valor único e imutável que pode ser usado como chave de propriedade de um objeto.
   ```javascript
   let simbolo1 = Symbol('descricao');
   let simbolo2 = Symbol('descricao');
   ```

Além desses, o JavaScript também possui tipos de dados mais avançados, como funções, que são objetos especiais, e outros tipos introduzidos em versões mais recentes da linguagem, como BigInt para representar inteiros grandes.

### - **O que são funções em JavaScript e como são criadas?**

Funções são blocos de código projetados para realizar uma tarefa específica ou calcular um valor. Elas são fundamentais para organizar, reutilizar e estruturar código de forma eficiente. Aqui estão algumas maneiras de criar funções em JavaScript:

1. **Declaração de Função (Function Declaration)**: Este é o método mais comum para declarar uma função. Uma função declarada dessa forma pode ser chamada antes de sua definição devido ao "hoisting" (elevação).

   ```javascript
   function saudacao(nome) {
       return `Olá, ${nome}!`;
   }
   
   console.log(saudacao('Maria')); // Saída: Olá, Maria!
   ```

2. **Expressão de Função (Function Expression)**: Neste método, a função é atribuída a uma variável. As funções declaradas dessa forma não são elevadas, então só podem ser chamadas após sua definição.

   ```javascript
   const saudacao = function(nome) {
       return `Olá, ${nome}!`;
   };
   
   console.log(saudacao('João')); // Saída: Olá, João!
   ```

3. **Arrow Function (Função de Seta)**: Introduzidas no ECMAScript 6 (ES6), as arrow functions fornecem uma sintaxe mais curta e lexicamente vinculam o `this` ao contexto onde a função foi definida.

   ```javascript
   const saudacao = (nome) => `Olá, ${nome}!`;
   
   console.log(saudacao('Ana')); // Saída: Olá, Ana!
   ```

4. **Funções Anônimas**: São funções sem nome, geralmente usadas como argumentos para outras funções ou como IIFE (Immediately Invoked Function Expressions).

   ```javascript
   // Como argumento de outra função
   setTimeout(function() {
       console.log('Essa mensagem aparece após 2 segundos.');
   }, 2000);

   // IIFE
   (function() {
       console.log('Essa função é executada imediatamente.');
   })();
   ```

5. **Funções de Classe (Métodos)**: Quando dentro de uma classe, funções são chamadas de métodos. Eles são declarados de maneira semelhante a funções regulares.

   ```javascript
   class Pessoa {
       constructor(nome) {
           this.nome = nome;
       }
       
       saudacao() {
           return `Olá, ${this.nome}!`;
       }
   }
   
   const pessoa = new Pessoa('Carlos');
   console.log(pessoa.saudacao()); // Saída: Olá, Carlos!
   ```

Cada um desses métodos de criação de funções tem suas particularidades e é útil em diferentes contextos dentro de um programa em JavaScript.

### 3) **JavaScript no Navegador:**
 
- **Como o JavaScript interage com HTML e CSS?**

 JavaScript interage com HTML e CSS de várias maneiras para criar páginas web dinâmicas e interativas:

1. **Manipulação do DOM (Document Object Model):**
   - **Selecionar elementos:** Usando métodos como `getElementById`, `querySelector`, etc.
   - **Alterar conteúdo:** Usando `innerHTML`, `textContent`, etc.
   - **Alterar estilos:** Modificando a propriedade `style` dos elementos.
   - **Adicionar/remover classes:** Usando `classList`.

2. **Manipulação de Eventos:**
   - Adicionando ouvintes de eventos para responder a cliques, movimentos do mouse, pressionamentos de teclas, etc.
   ```javascript
   document.getElementById('meuBotao').addEventListener('click', function() {
       alert('Botão clicado!');
   });
   ```

3. **Manipulação de CSS:**
   - Alterando regras de estilo diretamente.
   ```javascript
   document.getElementById('meuElemento').style.color = 'red';
   ```

4. **Integração com APIs do Navegador:**
   - **Geolocalização:** Para obter a localização do usuário.
   - **LocalStorage:** Para armazenar dados no navegador.
   ```javascript
   localStorage.setItem('chave', 'valor');
   const valor = localStorage.getItem('chave');
   ```

5. **Manipulação de Formulários:**
   - Validando e manipulando dados de formulários antes do envio.
   ```javascript
   document.getElementById('meuFormulario').addEventListener('submit', function(evento) {
       if (document.getElementById('meuInput').value === '') {
           evento.preventDefault();
           alert('O campo não pode estar vazio!');
       }
   });
   ```

Essas interações permitem criar páginas web mais dinâmicas, responsivas e interativas, melhorando a experiência do usuário.

### - **Pesquise sobre o DOM (Document Object Model) e sua relação com o JavaScript:**

O Document Object Model (DOM) é uma interface de programação que os navegadores implementam para representar documentos HTML e XML como uma estrutura de árvore, onde cada nó da árvore corresponde a uma parte do documento. O DOM permite que os desenvolvedores acessem, modifiquem e atualizem o conteúdo, a estrutura e o estilo de uma página de forma dinâmica usando JavaScript.

### Estrutura do DOM
A estrutura do DOM se assemelha a uma árvore, com nós que representam elementos HTML, atributos e texto. O nó raiz é geralmente o elemento `<html>`, com ramificações que incluem `<head>`, `<body>`, e assim por diante. Isso facilita a navegação e manipulação de diferentes partes do documento.

### Manipulação do DOM com JavaScript
JavaScript usa a API do DOM para manipular a árvore do DOM. Através do objeto `document`, os desenvolvedores podem selecionar elementos usando métodos como `getElementById`, `getElementsByClassName`, e `querySelector`, entre outros. Uma vez que um elemento é selecionado, suas propriedades e conteúdo podem ser modificados.

**Exemplo de seleção e modificação de um elemento:**
```javascript
const header = document.getElementById('header');
header.textContent = 'Novo título';
```

### Eventos e Interatividade
O DOM permite adicionar interatividade às páginas web através de eventos. Eventos como cliques, movimentos do mouse e pressionamentos de teclas podem ser capturados e manipulados com JavaScript. 

**Exemplo de manipulação de evento:**
```javascript
const button = document.getElementById('myButton');
button.addEventListener('click', function() {
  alert('Botão clicado!');
});
```

### Fases de Propagação de Eventos
Os eventos no DOM podem se propagar em duas fases: captura e bolha. Na fase de captura, o evento começa no elemento raiz e se move para o alvo. Na fase de bolha, o evento sobe do elemento alvo de volta ao elemento raiz. Isso permite um controle refinado sobre como os eventos são manipulados em estruturas de elementos aninhados.

### Relação com HTML e CSS
- **HTML:** Fornece a estrutura do documento, que é representada pela árvore do DOM.
- **CSS:** Define a apresentação visual dos elementos do DOM. JavaScript pode alterar as regras de estilo diretamente, permitindo uma atualização dinâmica da aparência da página.

### **Conclusão**
O DOM é crucial para a criação de páginas web interativas e dinâmicas. Ele fornece uma interface poderosa para ler, modificar e reagir a alterações na estrutura do documento.

### 4) **Ferramentas e Ambiente de Desenvolvimento:**
### - **Quais são algumas das ferramentas e ambientes que você pode usar para escrever e testar código JavaScript? (Exemplo: navegadores, editores de código como VS Code):**
Para escrever e testar código JavaScript, você pode usar várias ferramentas e ambientes:

### Navegadores
1. **Google Chrome Developer Tools**: Console interativo para escrever, depurar e testar código.
2. **Mozilla Firefox Developer Tools**: Similar ao Chrome, com ferramentas para depuração e análise.
3. **Microsoft Edge Developer Tools**: Baseado no Chromium, oferece ferramentas semelhantes ao Chrome.

### Editores de Código
1. **Visual Studio Code (VS Code)**: Editor popular com suporte para extensões como ESLint e Prettier.
2. **Sublime Text**: Leve e rápido, com suporte para plugins.
3. **Atom**: Altamente personalizável com muitos pacotes disponíveis.
4. **WebStorm**: IDE robusto para JavaScript, com suporte avançado para frameworks como React e Angular.

### Ambientes de Desenvolvimento
1. **Node.js**: Permite a execução de JavaScript no lado do servidor, com npm para gerenciamento de pacotes.
2. **CodePen**: Editor online para prototipagem rápida e compartilhamento de código.
3. **JSFiddle**: Ferramenta online para editar, executar e compartilhar código.
4. **Repl.it**: Plataforma online colaborativa para desenvolvimento em várias linguagens.

### Ferramentas de Linters e Formatadores
1. **ESLint**: Linter configurável para identificar e corrigir problemas em código JavaScript.
2. **Prettier**: Formatador de código que garante um estilo consistente.

Essas ferramentas ajudam a escrever, testar e depurar código JavaScript de maneira eficiente, facilitando o desenvolvimento de aplicações web dinâmicas.

### 5) **Recursos de Aprendizado:**

### - **Identifique e liste alguns recursos úteis para aprender JavaScript (sites, tutoriais, cursos online):**

Aqui estão alguns recursos úteis para aprender JavaScript:

### Sites e Tutoriais
1. **[MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)**
   - Documentação abrangente e tutoriais detalhados.
2. **[W3Schools](https://www.w3schools.com/js/)**
   - Tutoriais interativos e exemplos práticos.
3. **[JavaScript.info](https://javascript.info/)**
   - Tutorial completo desde conceitos básicos até avançados.
4. **[Codecademy](https://www.codecademy.com/learn/introduction-to-javascript)**
   - Cursos interativos com exercícios práticos.

### Cursos Online
1. **[freeCodeCamp](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/)**
   - Currículo completo e gratuito com exercícios e projetos práticos.
2. **[Coursera](https://www.coursera.org/courses?query=javascript)**
   - Cursos oferecidos por universidades e instituições renomadas.
3. **[Udemy](https://www.udemy.com/topic/javascript/)**
   - Vasta seleção de cursos pagos e gratuitos.
4. **[edX](https://www.edx.org/learn/javascript)**
   - Cursos de JavaScript por instituições como Harvard e MIT.

### Videos e Canais no YouTube
1. **[Traversy Media](https://www.youtube.com/user/TechGuyWeb)**
   - Tutoriais de desenvolvimento web.
2. **[The Net Ninja](https://www.youtube.com/c/TheNetNinja)**
   - Séries de tutoriais sobre JavaScript e frameworks associados.
3. **[Academind](https://www.youtube.com/c/Academind)**
   - Cursos detalhados sobre JavaScript e tecnologias web.

### Livros
1. **[Eloquent JavaScript](https://eloquentjavascript.net/)** por Marijn Haverbeke
   - Livro gratuito online que cobre JavaScript de forma profunda.
2. **[You Don’t Know JS (Yet)](https://github.com/getify/You-Dont-Know-JS)** por Kyle Simpson
   - Série de livros que aprofunda conceitos essenciais de JavaScript.

Esses recursos oferecem materiais educativos variados, desde tutoriais introdutórios até cursos avançados, ajudando você a aprender JavaScript de forma eficaz.



