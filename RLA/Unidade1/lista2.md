Q.1 Algoritmo Media

```java
DECLARE num1, num2, num3, num4, media: REAL

INICIO
    // Pede ao usuário que digite os números
    ESCREVA "Digite o número 1:"
    LEIA num1
    ESCREVA "Digite o número 2:"
    LEIA num2
    ESCREVA "Digite o número 3:"
    LEIA num3
    ESCREVA "Digite o número 4:"
    LEIA num4
    // Calcula a média dos números digitados
    media <- (num1 + num2 + num3 + num4) / 4
    // Mostre a média calculada
    ESCREVA "A média é ", media

FIM
```
Q.2 Algoritmo ConverteCelsiusFarenheit
DECLARE C, F: REAL

```java
INICIO
    // Pede ao usuário que digite a temperatura em Celsius
    ESCREVA "Digite a temperatura em Celsius:"
    // Le a temperatura em Celsius digitada pelo usuário
    LEIA C
    // Converte a temperatura de Celsius para Fahrenheit de forma diferente
    F <- (C * 9/5) + 32
    // Mostra a temperatura convertida em Fahrenheit
    ESCREVA "A temperatura em Fahrenheit é ", F, " graus"

FIM
```
Q.3 Algoritmo CalculadoraSimples

```java
DECLARE op: INTEIRO
DECLARE num1, num2, res: REAL

INICIO
    // Exibindo as operações válidas
    ESCREVA "Operações válidas: 1(soma), 2(subtração), 3(multiplicação) e 4(divisão)"

    // Solicitando ao usuário que digite uma operação
    ESCREVA "Digite uma operação:"
    LEIA op

    // Solicitando ao usuário que digite um número
    ESCREVA "Digite um número:"
    LEIA num1

    // Solicitando ao usuário que digite outro número
    ESCREVA "Digite outro número:"
    LEIA num2

    // Verificando a operação escolhida pelo usuário
    SE op == 1 ENTAO
        res <- num1 + num2
        ESCREVA num1, "+", num2, "=", res
    SENAO SE op == 2 ENTAO
        res <- num1 - num2
        ESCREVA num1, "-", num2, "=", res
    SENAO SE op == 3 ENTAO
        res <- num1 * num2
        ESCREVA num1, "*", num2, "=", res
    SENAO SE op == 4 ENTAO
        SE num2 != 0 ENTAO
            res <- num1 / num2
            ESCREVA num1, "/", num2, "=", res
        SENAO
            ESCREVA "Impossível dividir!"
        FIM_SE
    SENAO
        ESCREVA "Operação inválida!"
    FIM_SE

FIM
```
Q.4 Algoritmo ClassificaCategoria

```java
DECLARE idade: INTEIRO

INICIO
    // Pede ao usuário que insira a idade do aluno
    ESCREVA "Digite a idade do aluno:"
    // Lê a idade inserida pelo usuário
    LEIA idade
    // Verifica a idade e classificando nas categorias esportivas
    ESCOLHA
        // Verifica se a idade está na categoria Infantil A
        CASO idade >= 5 E idade <= 7
            ESCREVA "Infantil A"
        // Verifica se a idade está na categoria Infantil B
        CASO idade >= 8 E idade <= 10
            ESCREVA "Infantil B"
        // Verifica se a idade está na categoria Juvenil A
        CASO idade >= 11 E idade <= 13
            ESCREVA "Juvenil A"
        // Verifica se a idade está na categoria Juvenil B
        CASO idade >= 14 E idade <= 17
            ESCREVA "Juvenil B"
        // Verifica se a idade está na categoria Adulto
        CASO idade >= 18
            ESCREVA "Adulto"
        // Caso a idade não se encaixe em nenhuma categoria válida
        SENAO
            ESCREVA "Digite uma idade válida!"
    FIM_ESCOLHA

FIM
```
