# Sequência-de-Fibonacci
Sequência de Fibonacci

2 - Dado a sequência de Fibonacci, onde se inicia por 0 e 1 e o próximo valor sempre será a soma dos 2 valores anteriores (exemplo: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34...), escreva um programa na linguagem que desejar onde, informado um número, ele calcule a sequência de Fibonacci e retorne uma mensagem avisando se o número informado pertence ou não a sequência.

IMPORTANTE:

Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;

RESPOSTA: aqui está o código em JavaScript;  

function verificaFibonacci(numero) {
    let a = 0;
    let b = 1;
    while (b < numero) {
        const temp = b;
        b = a + b;
        a = temp;
    }
    return b === numero;
}

const numeroInformado = parseInt(prompt("Digite um número para verificar se pertence à sequência de Fibonacci:"));

if (verificaFibonacci(numeroInformado)) {
    console.log(`O número ${numeroInformado} pertence à sequência de Fibonacci.`);
} else {
    console.log(`O número ${numeroInformado} não pertence à sequência de Fibonacci.`);
}

/* Neste código JavaScript, a função verificaFibonacci() verifica se o número dado pertence à sequência de Fibonacci, utilizando uma abordagem iterativa semelhante à implementação em Python. Após a definição da função, o código solicita ao usuário que insira um número usando prompt(), converte esse valor para inteiro com parseInt(), e então chama a função verificaFibonacci() com esse número. Por fim, ele exibe uma mensagem no console indicando se o número pertence ou não à sequência de Fibonacci. */


