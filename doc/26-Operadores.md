# Operadores

  
  
&nbsp;
  
  
Existem cinco tipos de operadores no JavaScript, os **operadores aritméticos**, os **operadores de atribuição**, **operadores lógicos**, **operadores de comparação** e **operadores bitwise**.
  
  
&nbsp;
  
  
### Operadores aritméticos:
  
Os operadores aritméticos nos permitem realizar operações matemáticas no JavaScript.
  
  
| Operador | Descrição                                          |
|----------|----------------------------------------------------|
| +        | Soma                                               |
| -        | Subtração                                          |
| *        | Multiplicação                                      |
| **       | Exponenciação                                      |
| /        | Divisão                                            |
| %        | Módulo (resto da divisão de dois números inteiros) |
| ++       | Incremento                                         |
| --       | Decremento                                         |
  
  
```html
<script>
    var valor1 = 5;
    var valor2 = 10;
        
    var valor3 = "10";
    var resultado = valor1 + valor2;

    //OPERADORES ARITMÉTICOS

    //SOMA
    document.write(valor1 + " + " + valor2 + " = " + resultado + "<br>");

    //CONCATENAÇÃO
    document.write(valor1 + " CONC " + valor2 + " = " + valor1 + valor3 + "<br>");

    //SUBTRAÇÃO
    document.write(valor1 + " - " + valor2 + " = " + (valor1 - valor2) + "<br>");

    //MULTIPLICAÇÃO
    document.write(valor1 + " * " + valor2 + " = " + valor1 * valor2 + "<br>");

    //DIVISÃO
    document.write(valor1 + " / " + valor2 + " = " + valor1 / valor2 + "<br>");

    //MÓDULO
    document.write(valor1 + " % " + valor2 + " = " + valor2 % valor1 + "<br>");

    //EXPONENCIAÇÃO
    document.write(valor1 + " ** " + 2 + " = " + valor1 ** 2 + "<br>");

    //INCREMENTO
    document.write("valor1++" + valor1++ + "<br>");

    //DECREMENTO
    document.write("valor1--" +  valor2-- + "<br>");
</script>
```

  
  
&nbsp;
  
  
### Operadores de atribuição:
  
Os operadores de atribuição permitem atribuir valores às variáveis.
  
| Operador | Descrição                                                              |
|----------|------------------------------------------------------------------------|
| =        | Atribui o valor que está à direita à uma variável que está a esquerda. |
| +=       | Atribuição com atribuição                                              |
| -=       | Atribuição com subtração                                               |
| *=       | Atribuição com multiplicação                                           |
| /=       | Atribuição com divisão                                                 |
| %=       | Atribuição com módulo                                                  |
| ** **=**      | Atribuição com exponenciação                                           |
  
  
```html
<script>
    //OPERADORES DE ATRIBUIÇÃO

    //ATRIBUIÇÃO
    valor1 = valor2
    document.write(valor1 + "<br>");

    //ATRIBUIÇÃO COM SOMA
    valor1 += valor2
    document.write(valor1 + "<br>");

    //ATRIBUIÇÃO COM SUBTRAÇÃO
    valor1 -= valor2
    document.write(valor1 + "<br>");

    //ATRIBUIÇÃO COM MULTIPLICAÇÃO
    valor1 *= valor2
    document.write(valor1 + "<br>");

    //ATRIBUIÇÃO COM DIVISÃO
    valor1 /= valor2
    document.write(valor1 + "<br>");

    //ATRIBUIÇÃO COM MÓDULO
    valor1 %= 2
    document.write(valor1 + "<br>");

    //ATRIBUIÇÃO COM EXPONENCIAÇÃO
    valor1 **= 2
    document.write(valor1 + "<br>");
</script>
```

  
  
&nbsp;
  
  
[< Retornar à página principal](../README.md)
  
  
[Ir para a próxima página >]()
