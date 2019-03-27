# Caixas e mais caixas
  
  


  
&nbsp;
  
  
Vocês vão perceber com o passar do tempo que tudo no HTML e no CSS se resume a caixas. Muitos elementos HTML podem ser pensados desta forma, onde através do CSS conseguimos alterar seu tamanho, cor, posição, etc.
Cada uma dessas caixas ocupam um espaço dentro da página Web e possui propriedades que podem ser alteradas.
  
  
&nbsp;
  
  

## Elementos em bloco X elementos em linha
Há duas categorias importantes no HTML, que você precisa conhecer — elementos em bloco e elementos linha.
  
  
&nbsp;
  
  
### Elementos em bloco:
Formam um bloco visível na página. Eles aparecerão em uma nova linha logo após qualquer elemento que venha antes dele, e qualquer conteúdo depois de um elemento em bloco também aparecerá em uma nova linha. Elementos em bloco geralmente são elementos estruturais na página que representam, por exemplo: parágrafos, listas, menus de navegação, rodapés etc. Um elemento em bloco não seria aninhado dentro de um elemento inline, mas pode ser aninhado dentro de outro elemento em bloco.

```
<html>
  <body>
      <p>Primeiro parágrafo</p><p><em>Segundo parágrafo</em></p><p>Terceiro parágrafo</p>
  </body>
</html>
```
  
Os elementos de bloco possuem uma margem, uma borda e um pading.
  
  
Veja como isso é mostrado no navegador:
![Box Model](imagens/bloco.png)
  
  
&nbsp;
  
  
**Padding:** É o espaço entre o conteúdo e a borda do elemento;
![Padding](imagens/padding.png)
  
  
&nbsp;
  
  
**Margin:** É o espaço externo de uma caixa;
![Margin](imagens/margin.png)
  
  
**Border:** É a linha sólida do lado de fora ao redor da caixa;
  
  
&nbsp;
  
  
### Elementos inline (na linha):
São aqueles que estão contidos dentro de elementos em bloco, envolvem apenas pequenas partes do conteúdo do documento e não parágrafos inteiros ou agrupamentos de conteúdo. Um elemento inline não fará com que uma nova linha apareça no documento: os elementos inline geralmente aparecem dentro de um parágrafo de texto, por exemplo: um elemento \<a\>  (hyperlink) ou elementos de ênfase como \<em\> ou \<strong\>.

```
<hmtl>
  body>
      <p>
          <strong>Lorem ipsum dolor sit amet consectetur adipisicing elit.</strong> Eos corrupti distinctio consequuntur dolore sapiente rem <em>in odio facere hic nisi temporibus aut a,</em> asperiores repudiandae ipsum nihil esse veritatis totam.
      </p>
  </body>
</html>
```

  
  
&nbsp;
  
  
*Vamos ver algumas propriedades CSS que podemos utilizar para estilizar os elementos de texto e imagens.*

  
  
&nbsp;
  
  
[< Retornar à página principal](../README.md)
