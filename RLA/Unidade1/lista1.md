# Q.1 Algoritmo para determinar se um número inteiro e positivo é par ou impar

```java
ALGORITMO TrocaValores
DECLARE numero, resto: INTEIRO

INICIO
    //  Pede ao usuário que coloque um número
    ESCREVA "Digite um número: "
    // Lê o número colocado pelo usuário
    LEIA numero
    // Verifica se o número é positivo
    SE numero >= 0 ENTAO
        // Calcula o resto da divisão por 2 para determinar se é par ou ímpar
        resto <- numero % 2
        // Verifica se o resto da divisão é diferente de 0 (ímpar)
        SE resto != 0 ENTAO
            ESCREVA "O número é ímpar!"
        SENÃO
            ESCREVA "O número é par!"
        FIM_SE
    SENÃO             
        ESCREVA "O número deve ser positivo!"
    FIM_SE

FIM
```

Q.2 Algoritmo para calcular o novo salário de um funcionário

DECLARE sal_atual, sal_reaj: REAL

INICIO
    // Pede ao usuário que coloque seu salário atual
    ESCREVA "Digite seu salário atual:"
    // Lê o salário atual colocado pelo usuário
    LEIA sal_atual
    // Verifica o salário atual e colocando o reajuste de forma diferente
    SE sal_atual <= 500 ENTAO
        sal_reaj <- sal_atual * 1.2
    SENÃO
        sal_reajustado <- sal_atual * 1.15
    FIM_SE
    // Mostra o novo salário reajustado
    ESCREVA "O novo salário é R$", salario_reajustado

FIM

Q.3 Algoritmo para calcular a média aritmética entre duas notas de um aluno e mostrar sua situação, que pode ser aprovado ou reprovado

DECLARE nota1, nota2, media: REAL

INICIO
    // Pede ao usuário que coloque a nota 1
    ESCREVA "Digite a nota 1:"
    // Lê a nota 1 colocada pelo usuário
    LEIA nota1
    // Pede ao usuário que coloque a nota 2
    ESCREVA "Digite a nota 2:"
    // Lê a nota 2 colocada pelo usuário
    LEIA nota2
    // Verifica se as notas são maiores ou iguais a zero
    SE nota1 >= 0 E nota2 >= 0 ENTAO
        // Calcula a média das notas
        media <- (nota1 + nota2) / 2
        // Verifica se a média é maior ou igual a 7 para aprovação
        SE media >= 7 ENTAO
            ESCREVA "O aluno está aprovado!"
        SENÃO
            ESCREVA "O aluno está reprovado!"
        FIM_SE
    SENÃO
        ESCREVA "A nota deve ser maior que zero!"
    FIM_SE

FIM

Q.4 Algoritmo que determina se pode ou não tirar a CNH, a partir da idade do candidato. Caso não atender a restrição de idade, calcular quantos anos faltam para o candidato estar apto

DECLARE idade, anos_apto: INTEIRO

INICIO
    // Pede ao usuário que coloque sua idade
    ESCREVA "Digite a sua idade:"
    // Lê a idade colocada pelo usuário
    LEIA idade
    // Verifica se a idade é menor que zero
    SE idade < 0 ENTAO
        ESCREVA "A idade deve ser maior que zero!"
    // Verifica se a idade é maior ou igual a 18
    SENÃO
        SE idade >= 18 ENTAO
            ESCREVA "O candidato está apto a tirar a CNH!"
        SENÃO
            anos_apto <- 18 - idade
            ESCREVA "Faltam ", anos_apto, " anos para o candidato estar apto!"
        FIM_SE
    FIM_SE

FIM


