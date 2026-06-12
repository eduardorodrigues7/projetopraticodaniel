# Autômato de Pilha para Verificação de Parênteses Balanceados

## Disciplina

Teoria da Computabilidade

## Modelo Escolhido

Autômato de Pilha (Pushdown Automaton - PDA)

## Objetivo

Implementar um Autômato de Pilha capaz de reconhecer expressões contendo parênteses balanceados.

## Fundamentação Teórica

Um Autômato de Pilha é um modelo computacional composto por:

* Conjunto de estados
* Alfabeto de entrada
* Pilha
* Função de transição
* Estado inicial
* Estado(s) de aceitação

A principal diferença entre um Autômato Finito e um Autômato de Pilha é a presença da pilha, permitindo reconhecer linguagens livres de contexto.

## Problema Resolvido

Verificar se uma expressão possui parênteses corretamente balanceados.

Exemplos aceitos:

(())

((()))

()()

(()())

Exemplos rejeitados:

(()

))(

())(

## Funcionamento

1. Quando o símbolo '(' é encontrado, ele é empilhado.
2. Quando o símbolo ')' é encontrado, um elemento é removido da pilha.
3. Se for necessário remover um elemento de uma pilha vazia, a cadeia é rejeitada.
4. Ao final da leitura, a pilha deve estar vazia para que a cadeia seja aceita.

## Como Executar

python pda.py

## Exemplo

Entrada:

(()())

Saída:

CADEIA ACEITA
