# HTML BÁSICO
  
  
&nbsp;
  
  
O HTML é uma sigla que significa **H**yperText **M**arkup **L**anguage (Linguagem de Marcação de HiperTexto), ela serve para definir o conteúdo, estrutura e como as páginas serão mostradas nos browsers (Google Chrome, Opera, Firefox, Internet Explorer, entre outros) mas afinal o que significa **HTML**?

*OK, vamos por partes!*

**Hypertext** É um conceito antigo onde textos podem ser acessados de forma não linear a partir de qualquer ponto. Atualmente os textos disponibilizados na Web são compostos por nós e conexões que podem ser acessados de qualquer lugar. Os links que conectam uma página a outra, possibilitando a navegação entre páginas do mesmo site ou entre sites diferentes são exemplos de hipertextos. Afinal o principal objetivo da Web é conectar pessoas, quando criamos links entre páginas nos tornamos ativos na Internet e colaboramos para que ela cresça cada vez mais. 

**Markup** são como etiquetas utilizadas para falar ao browser como mostrar o conteúdo do site na tela do computador, celular, etc. Na verdade, não só isso! Existem tags especiais que não mostram nenhum conteúdo na tela, mas servem para estruturar o site.
Um exemplo de algumas tags que utilizamos \<html\>, \<head\>, \<body\> e \<p\>.
    
*Não se preocupem em entender para que elas servem agora, porque veremos em detalhes mais pra frente! =)*

**Language** nada mais é do que linguagem em inglês, ou seja, HTML é uma linguagem que utiliza etiquetas para criar a estrutura das páginas e links entre elas. 

*Fácil né? ;-)*
  
  
&nbsp;
  
## O que realmente é o HTML?

Muita gente pensa que o HTML é uma linguagem de programação, mas este é um pensamento equivocado. O HTML é na verdade uma linguagem de marcação, ele indica ao navegador que determinada parte da página é um título, ou parte do texto deve ser exibido em negrito, etc. É muito semelhante a forma de diagramação de livros, onde durante o processo de edição essas marcações são inseridas para indicar como o conteúdo será impresso.
Existem ainda muitos softwares que fazem isso, como por exemplo o Latex e o TextMaker. Repare nas tags escritas em vermelho e azul.

![Latex](imagens/latex.png)

O HTML segue o mesmo princípio, as tags servem para mostrar ao navegador como será apresentado o conteúdo do site.
  
  
&nbsp;
  
## Estrutura das TAGS

As tags são elementos escritos entre sinais de menor que (\<) e maior que (\>), se quisermos escrever um parágrafo por exemplo, utilizamos a tag \<p\>.
Para indicar o início do parágrafo utilizamos o \<p\> e para indicar o final utilizamos o \</p\>, todo o conteúdo do parágrafo deve ser escrito entre essas duas tags. Essa estrutura serve para a maioria das tags HTML.

```html
<html>
  <body>
    <p>Este é um exemplo de parágrafo, todo o conteúdo deve ser escrito aqui</p>
  </body>
</html>
```

As tags podem conter atributos que proveem informações adicionais sobre o conteúdo dos elementos. Eles aparecem dentro da tag de abertura e são compostos por duas partes **nome** e **valor**. 

```html
<html lang="en">
```

Repare que o valor é escrito entre “aspas” e eles são separados pelo sinal de igual ( = ). O nome do atributo indica que tipo de informação extra você está passando na tag, no exemplo acima estamos indicando que a linguagem da página será em Inglês. 
  
  
&nbsp;
  
## Tags vazias

Algumas tags não têm conteúdo, como no caso da tag \<img\>, ela serve para exibir imagens na página Web, contém apenas atributos e não precisa da tag de fechamento.

```html
<html>
  <body>
    <img src="img/minhaImagem.jpg" alt="Esta é uma imagem de exmplo">
  </body>
</html>
```
  
  
&nbsp;
  
## Estrutura da página HTML

Toda página HTML deve começar com a tag \<!DOCTYPE\>, ela mostra a versão da linguagem que será utilizada para criar a página Web, isso mesmo, existem versões diferentes da linguagem HTML, pois, novos recursos foram inseridos com o passar do tempo.

| Versão    | Ano  |
| ------    | ---  |
| HTML      | 1991 |
| HTML 2.0  | 1995 |
| HTML 3.2  | 1997 |
| HTML 4.01 | 1999 |
| XHTML     | 2000 |
| HTML 5    | 2014 |

O \<!DOCTYPE\> deve ser declarado apenas uma vez e deve ser a primeira tag da página. Neste caso, para indicarmos que a página será escrita em HTML 5 utilizamos:

```html
<!DOCTYPE html>
```

A tag <html> é conhecida como elemento raiz, e indica que tudo que está dentro dela é um conteúdo HTML. Lembram dos atributos que falamos agora a pouco na parte de Estrutura das TAGS? Então podemos ver sua utilização aqui! O atributo lang=”en” indica para o navegador que a página será escrita em Inglês.

```html
<html lang="en">
    Conteúdo HTML aqui
</html>
```

Veja mais códigos de linguagem: [W3Schools](https://www.w3schools.com/tags/ref_language_codes.asp)

A tag \<head\> contém informações adicionais sobre a página, como por exemplo, scripts que devem ser executados antes do carregamento da página, links para arquivos de estilo, formato de caracteres, título e muito mais. O seu conteúdo não é mostrado no navegador.

```html
<html>
  <head>
      <!-- Logo mais falaremos sobre as meta tags -->
      <meta charset="UTF-8">
      <title>Uma página muito bacana!</title>
  </head>
</html>
```

A tag \<body\> contém todo o conteúdo que você quer mostrar no navegador como textos, imagens, vídeos, etc.
    
```html
<html>
  <body>
      <h1>Hello World!</h1>
      <h2>Essa é a nossa primeira página</h2>
      <img src="img/minhaImagem.jpg" alt="Esta é uma imagem de exmplo">
  </body>
</html>
```

Então a estrutura final do nosso arquivo será assim:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
</head>
<body>
</body>
</html>
```
  
  
&nbsp;
  
## Criando arquivos .HTML

Para criar um arquivo HTML, no editor de texto que você escolheu para criar a sua página, basta clicar em **File / Save as…**, no nosso caso, estamos utilizando o VSCode como editor de texto.

![VSCode Save As](imagens/vscode_saveAs.png)
![VSCode Save](imagens/vscode_nomeArquivo.png)
  
  
&nbsp;
  
[< Retornar à página principal](../README.md)
  
  
[Ir para a próxima página >](3-Trabalhando-com-texto.md)

