# Curso - Web Designer</h1>
Escrito por: Cirilo Souza
Data da ultima atualização: 19/03/2019




## Convenções

Bom, antes de começarmos efetivamente, vamos a algumas convenções que usaremos aqui!

* Todos os exemplos de código serão mostrados desta forma;

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Uma página muito bacana!</title>
</head>
<body>

</body>
</html>
```

* O editor de texto que usamos para criar as páginas Web é o VSCode, existem vários no mercado e recomendo vocês darem uma pesquisada! O VSCode é da Microsoft e tem uma grande comunidade que contribui criando plug-ins para ele, então é uma boa pedida para quem está começando porque é simples e fácil de usar.
Para fazer o download, basta entrar no site do [Visual Studio](https://code.visualstudio.com/download).

* *Os meus comentários sempre serão escritos em itálico.*

*Acho que é isso! Vamos começar?*





## HTML Básico


O HTML é uma sigla que significa **H**yperText **M**arkup **L**anguage (Linguagem de Marcação de HiperTexto), ela serve para definir o conteúdo, estrutura e como as páginas serão mostradas nos browsers (Google Chrome, Opera, Firefox, Internet Explorer, entre outros) mas afinal o que significa **HTML**?

* OK, vamos por partes! *

**Hypertext** são os links entre páginas Web que conectam uma página na outra, mesmo quando criamos links para navegação entre páginas do mesmo site ou entre sites diferentes. Afinal o principal objetivo da Web é conectar pessoas, quando criamos links entre páginas nos tornamos ativos na Internet e colaboramos para que ela cresça cada vez mais. 

**Markup** são como etiquetas utilizadas para falar ao browser como mostrar o conteúdo do site na tela do computador, celular, etc. Na verdade, não só isso! Existem tags especiais que não mostram nenhum conteúdo na tela, mas servem para estruturar o site.
Um exemplo de algumas tags que utilizamos \<html\>, \<head\>, \<body\> e \<p\>.
    
*Não se preocupem em entender para que elas servem agora, porque veremos em detalhes mais pra frente! =)*

**Language** nada mais é do que linguagem em inglês, ou seja, HTML é uma linguagem que utiliza etiquetas para criar a estrutura das páginas e links entre elas. 

*Fácil né? ;-)*



### O que realmente é o HTML?

Muita gente pensa que o HTML é uma linguagem de programação, mas este é um pensamento equivocado. O HTML é na verdade uma linguagem de marcação, ele é baseado nas marcações que eram utilizadas para diagramar livros, durante o processo de edição essas marcações são colocadas para indicar como o conteúdo seria impresso.
Existem ainda muitos softwares que fazem isso, como por exemplo o Latex e o TextMaker. Repare nas tags escritas em vermelho e azul.

![Latex](/imagens/latex.png)

O HTML segue o mesmo princípio, as tags servem para mostrar ao navegador como será apresentado o conteúdo do site.




### Estrutura das TAGS

As tags são elementos escritos entre sinais de menor que (\<) e maior que (\>), se quisermos escrever um parágrafo por exemplo, utilizamos a tag \<p\>.
Para indicar o início do parágrafo utilizamos o \<p\> e para indicar o final utilizamos o \<\/p\>, todo o conteúdo do parágrafo deve ser escrito entre essas duas tags. Essa estrutura serve para a maioria das tags HTML.

```
<p>Este é um exemplo de parágrafo, todo o conteúdo deve ser escrito aqui</p>
```

As tags podem conter atributos que proveem informações adicionais sobre o conteúdo dos elementos. Eles aparecem dentro da tag de abertura e são compostos por duas partes **nome** e **valor**. 

```
<html lang="en">
```

Repare que o valor é escrito entre “aspas” e eles são separados pelo sinal de igual ( = ). O nome do atributo indica que tipo de informação extra você está passando na tag, no exemplo acima estamos indicando que a linguagem da página será em Inglês. 




### Tags vazias

Algumas tags não têm conteúdo, como no caso da tag \<img\>, ela serve para exibir imagens na página Web, contém apenas atributos e não precisa da tag de fechamento.

```
<img src="img/minhaImagem.jpg" alt="Esta é uma imagem de exmplo">
```



### Estrutura da página HTML

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

```
<!DOCTYPE html>
```

A tag <html> é conhecida como elemento raiz, e indica que tudo que está dentro dela é um conteúdo HTML. Lembram dos atributos que falamos agora a pouco na parte de Estrutura das TAGS? Então podemos ver sua utilização aqui! O atributo lang=”en” indica para o navegador que a página será escrita em Inglês.

```
<html lang="en">
    Conteúdo HTML aqui
</html>
```

Veja mais códigos de linguagem: [W3Schools](https://www.w3schools.com/tags/ref_language_codes.asp)

A tag \<head\> contém informações adicionais sobre a página, como por exemplo, scripts que devem ser executados antes do carregamento da página, links para arquivos de estilo, formato de caracteres, título e muito mais. O seu conteúdo não é mostrado no navegador.

```
<head>
    <!-- Logo mais falaremos sobre as meta tags -->
    <meta charset="UTF-8">
    <title>Uma página muito bacana!</title>
</head
```

A tag \<body\> contém todo o conteúdo que você quer mostrar no navegador como textos, imagens, vídeos, etc.
    
```
<body>
    <h1>Hello World!</h1>
    <h2>Essa é a nossa primeira página</h2>
    <img src="img/minhaImagem.jpg" alt="Esta é uma imagem de exmplo">
</body>
```

Então a estrutura final do nosso arquivo será assim:

```
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
</head>
<body>
</body>
</html>
```



### Criando arquivos .HTML

Para criar um arquivo HTML, no editor de texto que você escolheu para criar a sua página, basta clicar em **File / Save as…**, no nosso caso, estamos utilizando o VSCode como editor de texto.

![VSCode Save As](/imagens/vscode_saveAs.png)

![VSCode Save](/imagens/vscode_nomeArquivo.png)




## Trabalhando com texto

Quando criamos páginas Web nós adicionamos tags que são chamadas de elementos, esses **elementos** informam ao navegador o que deve ser exibido e como será exibido na tela. 
Nesta sessão, vamos ver em detalhes os elementos que são usados para inserir texto em páginas HTML. Estes elementos são divididos em duas partes, os **estruturais** e os **semânticos**, os estruturais servem para criar textos, como cabeçalhos e parágrafos já os semânticos provêm informações extras como dar ênfase ao texto. 

#### Cabeçalho:
O cabeçalho possui seis níveis, iniciando pelo \<h1\> e finalizando no <\h6\> sendo o \<h1\> utilizado para o título principal, por isso deve ser único e os demais podem se repetir ao longo da página. Os navegadores mostram o conteúdo dos cabeçalhos em tamanhos diferentes, de acordo com a sua ordem, ou seja, o <\h1\> será o maior e o <\h6\> o menor.

```
<body>
    <h1>Esse é um título em H1</h1>
    <h2>Esse é um título em H2</h2>
    <h3>Esse é um título em H3</h3>
    <h4>Esse é um título em H4</h4>
    <h5>Esse é um título em H5</h5>
    <h6>Esse é um título em H6</h6>
</body>
```

Veja como isso é mostrado no navegador:
![Cabeçalho](/imagens/cabecalho.png)


#### Parágrafo:
Para criar um parágrafo, utilizamos o elemento \<p\>, tudo que for escrito entre este elemento será mostrado em uma ou várias linhas dependendo o tamanho do texto. Por padrão o navegador mostra cada novo parágrafo em uma linha diferente.
    
```
<body>
    <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil suscipit nam accusamus laudantium minus quia veniam itaque eos nemo aperiam quo sit voluptate hic, obcaecati, doloribus odio recusandae excepturi. Nesciunt?
    </p>
    <p>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptas facere error, dolore ad quae iusto numquam ratione tempora similique iure quisquam placeat consequatur labore molestias! Labore assumenda sequi itaque deleniti.
    </p>
</body>
```

![Parágrafo](/imagens/paragrafo.png)


#### Bold e Itálico:
Para destacar uma parte do texto, podemos mostrá-los com a fonte em negrito ou itálico para fazer isso basta colocar o trecho do texto que queremos destacar entre os elementos \<b\> (negrito) e \<i\>  (itálico).

```
<body>
    <p>
        <b>Lorem ipsum dolor sit amet consectetur adipisicing elit.</b> Nihil suscipit nam accusamus laudantium minus quia veniam itaque eos nemo aperiam quo sit voluptate hic, obcaecati, doloribus odio recusandae excepturi. Nesciunt?
    </p>
    <p>
        <i>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</i> Voluptas facere error, dolore ad quae iusto numquam ratione tempora similique iure quisquam placeat consequatur labore molestias! Labore assumenda sequi itaque deleniti.
    </p>
</body>
```

![Negrito e Itálico](/imagens/negrito_italico.png)


#### Quebra de linha:
Utilizamos o elemento <br> para quebrar parte do texto em uma nova linha.

```
<p>
    <b>Lorem ipsum dolor sit amet <br>consectetur adipisicing elit.</b> Nihil suscipit nam accusamus laudantium minus quia veniam itaque eos nemo aperiam quo sit voluptate hic, obcaecati, doloribus odio recusandae excepturi. Nesciunt?
</p>
```

![Quebra de Linha](/imagens/quebra_de_linha.png)


#### Quebra de sessão:
Para separar sessões diferentes, ou parágrafos diferentes podemos utilizar o elemento \<hr\>. Ele cria uma linha que serve para separar um conteúdo de outro.

```
<body>
    <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aliquid inventore odit ducimus doloribus fugit eius quis deserunt ipsa obcaecati animi nisi recusandae id minima, asperiores quia, tenetur ex tempore corrupti?
    </p>
    <hr>
    <p>
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quae quia nulla quibusdam sunt corporis earum. Veniam eos tenetur, asperiores earum eaque officia. Perspiciatis earum praesentium veritatis, sit enim blanditiis exercitationem?
    </p>
</body>
```

![Quebra de sessão](/imagens/quebra_de_sessao.png)


#### Texto pré-formatado:
Geralmente quando queremos apresentar poemas, ou linhas de código de alguma linguagem de programação em uma página utilizamos o elemento \<pre\>.

```
<pre>
    Batatinha quando nasce
    Espalha a rama pelo chão
    Menininha quando dorme 
    Põe a mão no coração
</pre>
```


#### Sub escrito e sobre escrito:
O elemento \<sub\> (sub escrito) geralmente é usado para formulas químicas, como H2O.

```
<body>
    <p>A fórmula da água é H<sub>2</sub>O</p>
    <p>Qual o resultado de 2<sup>2</sup>?</p>
</body>
```


