# Um pouco mais de HTML
  
  
&nbsp;
  
  
No início deste material nós falamos bem rapidamente sobre o elemento \<head\>. Vamos entende-lo um pouco mais afundo agora que nós já temos mais experiência com HMTL.
O \<head\> é um container onde inserimos informações relevantes para o navegador, (estas informações não são exibidas na página web). Nele podemos inserir outros elementos que fornecem informações importantes à página web, como \<meta\>, \<link\>, \<style\>, \<scritp\>, etc.

  
  
&nbsp;
  
  
## Elemento \<meta\>
  
  
&nbsp;
  
  
O elemento \<meta\> pode possuir diversos atributos, como o charset, que define um conjunto de caracteres (letras, números, acentos, etc), ou seja, ele transforma os caracteres em códigos que o computador consegue entender. O valor UTF-8 cobre a maior parte dos caracteres existentes nas línguas ocidentais.

Somente a título de curiosidade, a palavra “Olá” em código de máquina seria assim: 

01101000 01100101 01101100 01101100 01101111

Isso é o que chamamos de código binário, porque é composto de apenas dois números 0 e 1. Não se preocupe em entender como funciona um código binário pois este não é o foco deste curso, mas se quiser saber um pouco mais sobre o UTF-8, você pode acessar o link abaixo:
  
  
[W3Schools](https://www.w3schools.com/charsets/ref_html_utf8.asp)

  
  
&nbsp;
  
  
### Descrição da página:

O atributo name=”description” é útil para descrever o conteúdo da sua página web, ele é utilizado pelos robôs de busca do Google, Bing, etc, para entender do que se trata a sua página. Utilizamos juntamente o atributo content, no qual inserimos o texto de descrição.  

```html
<meta name="description" content="Uma página muito bacana">
```

### Palavras chaves para robôs de busca:

Outro atributo muito usado é o name=”keywords”, onde informamos quais palavras chave os buscadores utilizarão para encontrar e mostrar o nosso site para os usuários na Internet.

```html
<meta name="keywords" content="HTML, CSS, XML, JavaScript">
```

### Autor da página:

O atributo name=”author” serve para informarmos quem criou a página web.

```html
<meta name="author" content="Fulano de Tal">
```

### Visualização da página:

O HTML5 introduziu o atributo name=”viewport”, ele é de extrema importância, pois, a nossa página pode ser vista em vários tipos de dispositivos (#spoiler), como computadores, notebooks, tablets, smartfones, etc. E estes dispositivos possuem tamanhos de tela diferentes, nossa página deve ser mostrada corretamente em cada um deles isso é o que chamamos de páginas responsivas.
  
  
[Página UOL](imagens/uol2.png)
  
  
[Página UOL Responsiva](imagens/uol3.png)
  
  
&nbsp;
  
  
[< Retornar à página principal](../README.md)
  
  
[Ir para a próxima página >](17-Páginas-Responsivas.md)
