# Operadores

  
  
&nbsp;
  
  
Existem cinco tipos de operadores no JavaScript, os operadores aritméticos, os operadores de atribuição e operadores lógicos, operadores de comparação e operadores bitwise.
  
  
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
  
  
[< Retornar à página principal](../README.md)
  
  
[Ir para a próxima página >]()
