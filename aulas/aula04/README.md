# Aula 4 — Estruturas Condicionais 🚦

## 🎯 Estrutura `if` / `else`
A estrutura condicional (`se / senão`) permite que o programa tome decisões com base em condições lógicas.
```c
if (condição) {
    // Código se a condição for VERDADEIRA
} else {
    // Código se a condição for FALSA
}
```

---

## 🏛️ Operadores Relacionais
As condições no `if` usam operadores relacionais:
*   `>`: Maior que.
*   `<`: Menor que.
*   `>=`: Maior ou igual a.
*   `<=`: Menor ou igual a.
*   `==`: Igual a (cuidado: um sinal de `=` é atribuição).
*   `!=`: Diferente de.

### Exemplo: Teste Simples
```c
int idade;
scanf("%d", &idade);
if (idade >= 18) {
    printf("Você é maior de idade!");
} else {
    printf("Você é menor de idade!");
}
```

---

## 📜 Estruturas Aninhadas (`if else if`)
Quando temos mais de duas opções, usamos o `else if`.
```c
if (nota >= 7) {
    printf("Aprovado");
} else if (nota >= 5) {
    printf("Recuperação");
} else {
    printf("Reprovado");
}
```

---

## 🏋️ Exercícios Práticos
### 1. Par ou Ímpar?
Crie um programa que leia um número inteiro e diga se ele é par ou ímpar (Dica: Use o operador de módulo `% 2 == 0`).

### 2. Aprovação de Aluno
Um aluno é aprovado se tiver média maior ou igual a 7. Se for entre 5 e 6.9, ele está de recuperação. Menor que 5, ele está reprovado. Peça a média ao usuário e informe a situação.

### 3. Maior de Três
Peça três números inteiros ao usuário e exiba qual é o maior deles na tela. Cuidado com números iguais!

---

## 💡 Dica da Aula: Indentação
Mantenha o código dentro das chaves (`{ }`) um pouco mais à direita (tecla **TAB**). Isso ajuda a ler e entender o que pertence a cada bloco.
