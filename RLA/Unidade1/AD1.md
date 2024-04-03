
Q.1 Algoritmo TrocaValores

```java
Declare a,b,aux: REAL
INICIO
    // Pede ao usuário para digitar o valor de 'a'
    ESCREVA "Digite o valor de a:"
    // Lê o valor de 'a' fornecido pelo usuário
    LEIA a
    // Pede ao usuário para digitar o valor de 'b'
    ESCREVA "Digite o valor de b:"
    // Lê o valor de 'b' fornecido pelo usuário
    LEIA b
    // Guarde o valor de'a' temporariamente em 'aux'
    aux <- a 
    // Atribui o valor de 'b' a 'a'
    a <- b
    // Restaura o valor original de 'a' armazenado em 'aux' a 'b'
    b <- aux

    // Mostra o valor atual de 'a' depois da  troca
    ESCREVA "a = ", a

    // Mostra o valor atual de 'b' depois da  troca
    ESCREVA "b = ", b
FIM
```
Q.2 Algoritmo ContaAprovacoes

```java
Declare n, cont, nota, i: INTEIRO

INICIO

    // Pede ao usuário  para digitar a quantidade de notas dos alunos
    ESCREVA "Digite a quantidade de notas dos alunos:"

    // Lê a quantidade de notas dos alunos fornecida pelo usuário
    LEIA n

    // Inicia o contador de alunos aprovados
    cont = 0 

    // Loop para conseguir as notas dos alunos e passar os aprovados
    PARA i DE 1 ATE n FAÇA

        // Pede ao usuário que digite a nota do aluno
        ESCREVA "Digite a nota do aluno ", i, ":"

        // Lê a nota do aluno fornecida pelo usuário
        LEIA nota

        // Verifica se a nota está no intervalo de aprovação
        SE nota >= 50 E nota <= 100 então

            // Complementa o contador de alunos aprovados
            cont = cont + 1 

   FIM_SE

    FIM_PARA

FIM
```
Q.3. Algoritmo SomaNumeros

```java
DECLARE n, cont, nota, i: INTEIRO

INICIO

    // Pede ao usuário para digitar a quantidade de notas dos alunos
    ESCREVA "Digite a quantidade de notas dos alunos:"

    // Lê a quantidade de notas dos alunos fornecida pelo usuário
    LEIA n

    // Inicia o contador de alunos aprovados
    cont = 0 

    // Loop para obter as notas dos alunos e contar os aprovados
    PARA i DE 1 ATE n FAÇA

        // Pede ao usuário que digite a nota do aluno
        ESCREVA "Digite a nota do aluno ", i, ":"

        // Lê a nota do aluno fornecida pelo usuário
        LEIA nota

        // Verifica se a nota está no intervalo de aprovação
        SE nota >= 50 E nota <= 100 ENTAO

            // Complementa  o contador de alunos aprovados
            cont = cont + 1 
FIM usando SE

    FIM usando PARA

    // Mostra o número de alunos aprovados
    ESCREVA "O número de alunos aprovados é:", cont

FIM
```
Q.4 Algoritmo SomaSerie

```java
DECLARE n, numerador, denominador: INTEIRO
DECLARE termo, S: REAL

INICIO

    // Pede ao usuário para digitar o número de termos da série S
    ESCREVA "Digite o número de termos da série S:"

    // Lê o número de termos fornecido pelo usuário
    LEIA n

    // Inicia a soma da série S
    S <- 0

    // Loop para calcular os termos da série e somá-los
    PARA i DE 0 ATÉ n-1 PASSO 1 FAÇA

        // Calcula o numerador do termo atual
        numerador <- 2 * i + 1

        // Calcula o denominador do termo atual
        denominador <- 2 * i + 2

        // Calcula o termo atual da série
        termo <- numerador / denominador

        // Adiciona o termo atual à soma da série
        S <- S + termo

    FIM usando PARA

    // Mostra a soma da série S
    ESCREVA "Soma da série S é ", S

FIM
```
Q.5 Algoritmo CalcFatorial 

```java
DECLARE n: INTEIRO

INICIO

    // Coloque seu comentário
    ESCREVA "Digite um numero inteiro nao-negativo:"

    // Coloque seu comentário
    LEIA n

    // Coloque  seu comentário
    SE n >= 0 ENTAO

        // Coloque seu comentário
        fator <- 1

        // Coloque seu comentário
        PARA i DE 1 ATÉ n PASSO 1 FAÇA

            // Coloque seu comentário
            fator <- fator * i        // fator *= i

        FIM usando PARA

        // Coloque seu comentário
        ESCREVA "O fatorial de, n, é:", fator

    // Coloque seu comentário
    SENAO
        ESCREVA "O valor deve ser maior ou igual a zero!"
    FIM usando SE

FIM
```
Q.6 Algoritmo GeraFibonacci 

```java
DECLARE n, a, b, termo_atual: INTEIRO

INICIO

    // Pede ao usuário o número de termos da série Fibonacci
    ESCREVA "Número de termos da série Fibonacci:"
    // Lê o número de termos fornecido pelo usuário
    LEIA n
    // Inicia os dois primeiros termos da série
    a <- 0
    b <- 1
    // Loop para gerar os termos da série Fibonacci
    PARA i DE 1 ATE n FAÇA
        // Mostra o termo atual da série
        ESCREVA a
        // Calcula o próximo termo da série
        termo_atual <- a + b
        // Atualiza os valores de 'a' e 'b' para os próximos cálculos
        a <- b
        b <- termo_atual

    FIM usando o PARA

FIM
```
Q.7 Algoritmo InverteInteiro

```java
DECLARE num, num_inv, digito: INTEIRO

INICIO

    // Pede ao usuário que digite o número a ser invertido
    ESCREVA "Digite o número a ser invertido:"
    LEIA num
    // Verifica se o número é negativo
    SE num < 0 ENTAO
        // Se o número for negativo, exibe uma mensagem de erro
        ESCREVA "O número deve ser positivo!"
    // Se o número for positivo
    SENAO
        // Inicia o número invertido como zero
        num_inv <- 0
        // Enquanto o número original for maior que zero
        ENQUANTO num > 0 FAÇA
            // Adquiri o último dígito do número original
            digito <- num % 10
            // Adiciona o dígito à direita no número invertido
            num_inv <- (num_inv * 10) + digito
            // Remove o último dígito do número original
            num <- num / 10
        // Mostra o número invertido
        ESCREVA "Número invertido:", num_inv

    FIM_SE

FIM
```
