# Introdução ao JavaScript
  
  
&nbsp;
  
  
O JavaScript é uma linguagem de programação criada em 1995 por Brendan Eich co-fundador do projeto Mozilla para criar interações dinâmicas páginas web, como por exemplo ações que o site deve executar ao clicarmos em um botão, ou efeitos visuais que devem ocorrer após o carregamento da página, etc.
  
  
O JavaScript tem esse nome por causa de outra linguagem bem famosa na época, o Java. Mas é importante não confundirmos uma com a outra porque suas semelhanças param por aí. O Java é uma linguagem **compilada**, ou seja, nós desenvolvemos a aplicação em uma linguagem que nós humanos conseguimos entender e ao ser compilado, um arquivo é salvo com uma linguagem que as máquinas conseguem entender se houver algum erro no desenvolvimento, ele é detectado durante a compilação.
Já o JavaScript não passa por esse processo de compilação, porque todo o código é interpretado pelo navegador que se responsabiliza por transformar isso em algo que as máquinas consigam entender, se houver um erro no desenvolvimento do código ele será pego em tempo de execução. Chamamos isso de linguagem **interpretada**.
  
  
Em 1996 o JavaScript passou a ser “administrado” pela **ECMA (European Computer Manufacturers Association)** uma organização internacional que reúne grandes empresas de tecnologia e em 1997 foi lançada a primeira versão chamada **ECMAScript**.  De lá pra cá novas características foram adicionadas a linguagem que se tornou cada vez mais robusta.
  
  
Originalmente o Javascript foi concebido para funcionar apenas do lado do cliente (client side), em aplicações que são executadas somente nas máquinas dos usuários (smartphones, laptops, smart watches, etc). Mas a linguagem caiu no gosto dos desenvolvedores e passou a ser utilizada também em aplicações cliente servidor, como por exemplo o Node.JS.
Hoje o ECMAScript (*carinhosamente chamado por mim de JavaScript*) está na 9º edição e possui diversos recursos novos, vamos ver alguns deles aqui, mas se você quiser saber mais, recomendo ler a especificação no site da [ECMA](http://www.ecma-international.org/ecma-262/9.0/index.html#sec-intro).
  
  
&nbsp;
  
  
## Adicionando JavaScript a página web
  
  
&nbsp;
  
  

Vamos criar a nossa primeira interação com o JavaScript. O elemento <script> permite inserirmos linhas de código JavaScript diretamente na página web como acontece com o CSS, o JavaScript (JS como chamaremos de agora em diante) possui três formas de ser vinculado a página, interno, externo e in-line.
  
  
### Interno:
  
Todo o conteúdo que é escrito dentro do elemento <script> é interpretado pelo navegador como linguagem de script.
  
```html
    <script>
        document.getElementById('btn').onclick = mostraTexto;

        function mostraTexto(){
            document.getElementById('root').innerHTML = "Hello World!";
        }
    </script>
```
  
  
&nbsp;
  
  
### Externo:
  
Para utilizarmos um arquivo externo, basta adicionarmos o atributo src ao elemento script direcionando para o arquivo .js.

```html
    <script src="animation.js"></script>
```

Feito isso, temos que criar um arquivo com a extensão .JS (essa extensão indica ao navegador que este é um arquivo de código JavaScript), no exemplo acima, estamos criando um arquivo com o nome animation.js.
No arquivo JS, basta escrevermos o seguinte código.

```javascript
document.getElementById('btn').onclick = mostraTexto;

function mostraTexto(){
    document.getElementById('root').innerHTML = "Hello World!";
}
```

Repare que o mesmo código do exemplo anterior, porém no arquivo JS não utilizamos as tags \<script\>.
  
  
&nbsp;
  
  
### In-line:
  
```html
  <body>
      <h1>Olha só como é fácil programar em JavaScript!</h1>
      <h2 id="root"></h2>

      <button onclick="document.getElementById('root').innerHTML = 'Hello World!'">Clique me!</button>
  </body>
```
  
  
Nos exemplos de JS interno e externo, nós precisamos informar ao navegador quem era o \<button\> e quem era o \<h2\> através do atributo id. Já no exemplo de código in-line, não houve essa necessidade porque o código JS está sendo aplicado diretamente no botão, neste caso nós precisamos apenas informar que é o elemento \<h2\>.
  
  
&nbsp;
  
  
*Não entendeu o que está acontecendo? Não se preocupe, nós falaremos mais afundo o que cada parte deste código significa mais adiante! 
O importante até aqui é entendermos como podemos inserir os códigos JavaScript na nossa página Web.*

  
  
&nbsp;
  
  
## O que é um script?
  
  
&nbsp;
  
  
Por si só o JS não consegue fazer nada sozinho, ele precisa que nós informemos a ele o que deve fazer, ou seja, funciona como um roteiro, com uma série de instruções para criarmos algo. Como por exemplo uma receita de bolo ou um manual de instruções. 
Nos exemplos acima nós demos algumas instruções ao navegador, como por exemplo, capturar o evento de clique onclick do mouse sobre o botão, inserir o “Hello World” dentro da tag \<h2\> através do seu atributo id, tudo isso fomos nós que “falamos” para o JS fazer seguindo uma ordem lógica.
  
  
&nbsp;
  
  
[< Retornar à página principal](../README.md)
  
  
[Ir para a próxima página >](./25-O-que-sao-variaveis.md)
