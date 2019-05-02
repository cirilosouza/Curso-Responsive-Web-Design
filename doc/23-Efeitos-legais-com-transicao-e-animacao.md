# Adicionando efeitos visuais
  
  
&nbsp;
  
  
As transformações, transições e animações, permitem adicionar efeitos visuais aos elementos da página Web de forma que eles possam se movimentar na tela, ou interagir de acordo com um evento iniciado pelo usuário. Isso vai dar a nossa página Web um ar mais moderno, algo mais… “Descolado” (bem diferente das páginas estáticas). 


## Transformação 2D
  
  
&nbsp;
  
  
A propriedade CSS transform, nos permite mudar a forma e a posição de um elemento. Podemos rotacioná-los, movê-los e redimensioná-los em resposta a uma ação do usuário. O elemento sai do ponto A para o ponto B, ou seja, ele pode ter um tamanho inicial diferente do final, ou uma posição inicial diferente da final.
A propriedade transform possui os seguintes métodos:
  
  
| Valor        | Para que serve                                              |
|--------------|-------------------------------------------------------------|
| translate( ) | Move um elemento nos eixos X e Y.                           |
| rotate( )    | Rotaciona um elemento no sentido horário e anti-horário.    |
| scale( )     | Aumenta ou diminui o tamanho do elemento.                   |
| skewX( )     | Inclina um elemento no eixo X.                              |
| skewY( )     | Inclina um elemento no eixo Y.                              |
| matrix()     | Combina todos os valores anterios de transform em um único. |
  
  
&nbsp;
  
  
### Translate( ):
  
O valor translate() move um elemento de acordo com os eixos X e Y.
  
  
```css
.transform:hover{
    -ms-transform: translate(50px, 50px); /* IE 9 */
    -webkit-transform: translate(50px, 50px); /* Safari */
    transform: translate(50px, 50px);
}
```
  
  
Neste caso, estamos informando ao navegador que quando o usuário passar o mouse sobre o elemento (hover) queremos movê-lo 50px para a direita e 50px para baixo. 
  
  
![Transform](imagens/transform.gif)

  
  
&nbsp;
  
  
[< Retornar à página principal](../README.md)
  
  
[Ir para a próxima página >]()
