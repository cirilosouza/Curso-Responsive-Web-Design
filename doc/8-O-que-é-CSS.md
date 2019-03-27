# O que é CSS?
  
  
CSS significa Cascading Style Sheet, tá bom… isso não ajudou muito né?  ¯\\\_(ツ)\_/¯.
Assim como o HTML, o CSS também não é uma linguagem de programação, mas sim uma folha de estilos. Ele serve para informar ao navegador como os elementos devem ser apresentados na tela, papel, ou qualquer outro meio no qual a página possa ser vista. Ele nos ajuda a economizar um monte de trabalho porque podemos usar o mesmo estilo para vários elementos diferentes.
O estilo pode ser adicionado de três formas, in-line (no próprio elemento HTML), interno e externo.
  
  
&nbsp;
  
  
### Estilo in-line:
O estilo é aplicado no próprio elemento HTML e serve apenas para aquele elemento. 

```
<html>
  <body>
      <p style="color: red;">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur veniam praesentium nostrum facere vel. Esse ipsum maiores officia fuga. Perspiciatis saepe ab culpa quisquam aspernatur reprehenderit dolorem rem consequatur quibusdam.
      </p>
      <p style="color: blue;">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere quia sequi culpa libero quo exercitationem soluta fugiat sint, perspiciatis quae eos atque odit ut hic. Corrupti cupiditate animi iusto minus!
      </p>
  </body>
</html>
```
  
  
![Estilo inline](imagens/estilo_inline.png)
  
  
&nbsp;
  
  
### Estilo interno:
É aplicado através do elemento <style> dentro da página HTML.
  
```
<html>
  <head>
      <style>
          p{ color: green; }
      </style>
  </head>
  <body>
      <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur veniam praesentium nostrum facere vel. Esse ipsum maiores officia fuga. Perspiciatis saepe ab culpa quisquam aspernatur reprehenderit dolorem rem consequatur quibusdam.
      </p>
  </body>
</html>
```
  
  
![Estilo interno](imagens/estilo_interno.png)
  
  
Particularmente não recomendo aplicar estilos in-line e interno, porque conforme as páginas crescem se torna muito difícil dar manutenção neste tipo de código.
  
  
&nbsp;
  
  
### Estilo externo:
Para utilizarmos um arquivo CSS externo basta inserir elemento \<link\> dentro de \<head\> e no atributo rel informamos o valor “stylesheet” ou seja, uma folha de estilos. Não confunda o elemento \<link\> com as âncoras \<a\> que falamos agora a pouco.
Para finalizar, basta atribuir ao atributo href a localização do arquivo CSS.

```
<html>
  <head>
      <link rel="stylesheet" href="style.css">
  </head>
</html>
```
  
  
&nbsp;
  
  
## Anatomia do seletor CSS
  
  
![Seletor CSS](imagens/anatomia_do_seletor.png)
  
  
### Seletores (Selector):
Os seletores servem para selecionar os elementos HTML que queremos aplicar um estilo, existem diferentes tipos de seletores, por hora, veremos apenas três deles, seletor de elemento, ID e de classe.
  
  
| Nome do Seletor      | O que ele seleciona                         | Exemplo           |
| ----                 | ------                                      | -----             |
| Seletor de elemento  | Seleciona todos os elementos HTML da página | p{ color: red; }  | 
| Seletor de ID        | Seleciona um elemento específico através do seu atributo id. O ID é aplicado através do uso da hashtag # no arquivo CSS | <!—- Arquivo HTML -->
<body>
    <p id="paragrafo">Isso é um parágrafo</p>
</body>

<!—- Arquivo CSS -->
#paragrafo{
    color: red;
} | 

[< Retornar à página principal](../README.md)
