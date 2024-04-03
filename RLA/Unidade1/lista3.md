Q.1 Algoritmo verifica_par_impar

```java
DECLARE num, resto: INTEIRO

INICIO
    // Pede ao usuário que digite um número inteiro
    ESCREVA "Digite um número: "
    LEIA num
    // Verifica se o número é negativo e solicitando um número positivo
    ENQUANTO num < 0 FAÇA
        ESCREVA "Digite um número maior ou igual a zero:"
        LEIA num
    FIM_ENQUANTO
    // Verifica se o número é positivo
    SE num >= 0 ENTAO
        // Calcula o resto da divisão por 2 para determinar se é par ou ímpar
        resto <- num % 2
        // Verifica se o resto da divisão é igual a 0 (par) ou não (ímpar)
        SE resto == 0 ENTAO
            ESCREVA "O número é par!"
        SENAO
            ESCREVA "O número é ímpar!"
        FIM_SE
    // Mostra mensagem se o número não for positivo
    SENAO
        ESCREVA "O número deve ser positivo!"
    FIM_SE

FIM
```
Q.2 Algoritmo MultiploTres

```java
DECLARE n: INTEIRO

INICIO
    // Pede ao usuário que digite a quantidade de números
    ESCREVA "Digite a quantidade de números:"
    LEIA n
    // Loop contado (loop for) para exibir os números de 0 até n-1, adicionando de 3 em 3
    PARA i DE 0 ATÉ n-1 PASSO 3 FAÇA
        // Mostra o valor de i em cada iteração
        ESCREVA i
    FIM_PARA

FIM
```
Q.3 Algoritmo SomaValores

```java
ECLARE n, i: INTEIRO
DECLARE soma, num: REAL

INICIO
    // Pede ao usuário que digite a quantidade de números
    ESCREVA "Digite a quantidade de números:"
    LEIA n
    // Inicializa a variável soma com 0
    soma <- 0
    // Inicializa a variável i com 1
    i <- 1
    // Loop contado (loop for) para somar os números inseridos
    PARA i DE 1 ATÉ n FAÇA
        // Pede ao usuário que digite o número
        ESCREVA "Digite o número ", i, :"
        LEIA num
        // Somando o número inserido à variável soma
        soma <- soma + num
    FIM_PARA
    // Mostrando a soma dos números inseridos
    ESCREVA "A soma dos números é ", soma

FIM
```
Q.4 Algoritmo QuantMedia

```java
DECLARE nota, soma, media: REAL
DECLARE cont: INTEIRO

INICIO
    // Pede ao usuário que digite a nota do aluno (nota negativa finaliza)
    ESCREVA "Digite a nota do aluno (nota negativa finaliza): "
    // Armazenando o valor de entrada na variável "nota"
    LEIA nota
    // Inicializa as variáveis soma e cont
    soma <- 0
    cont <- 0
    // Loop condicional para executar as instruções até que a nota seja negativa
    ENQUANTO nota >= 0 FAÇA
        // Aumenta a nota à variável soma a cada iteração
        soma <- soma + nota
        // Incrementando em 1 na variável cont a cada iteração
        cont <- cont + 1
        // Pede a nota do próximo aluno (nota negativa finaliza)
        ESCREVA "Digite a nota do aluno (nota negativa finaliza): "
        LEIA nota
    FIM_ENQUANTO
    // Verifica se há notas para calcular a média
    SE cont > 0 ENTAO
        // Calcula a média das notas dos alunos
        media <- soma / cont
        // Mostra o número de notas lidas e a média aritmética
        ESCREVA "Foram lidas ", cont, " nota(s). A média aritmética é ", media
    FIM_SE

FIM
```
