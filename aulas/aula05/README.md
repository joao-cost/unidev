# Aula 5 — Estruturas de Repetição 🔁

## 🎯 Estruturas de Repetição (Loops)
Estruturas de repetição permitem executar o mesmo bloco de código várias vezes, poupando esforço e código. Em C, temos duas mais conhecidas:
1.  **`for`**: Usado quando sabemos quantas vezes repetiremos.
2.  **`while`**: Usado quando repetiremos enquanto uma condição for verdadeira.

---

## 🏛️ Loop `for`
Estrutura: `for (inicio; condição; incremento)`
```c
for (int i = 0; i < 5; i = i + 1) {
    printf("%d", i); // Mostrará 0, 1, 2, 3, 4
}
```

---

## 📜 Loop `while`
Estrutura: `while (condição)`
```c
int i = 0;
while (i < 5) {
    printf("%d", i);
    i = i + 1; // Importante atualizar o contador!
}
```

---

## 🏋️ Exercícios Práticos
### 1. Contar Números
Crie um programa que peça um número inicial e um número final ao usuário. O programa deve mostrar todos os números nesse intervalo de 1 em 1.

### 2. Tabuada
Peça ao usuário um número e mostre a tabuada dele de 1 a 10 (ex: 5 x 1 = 5, 5 x 2 = 10, ...).

### 3. Soma de Vários Números
Crie um programa que peça 5 números ao usuário, some todos eles e mostre o resultado final fora do loop.

### 4. Desafio: Jogo de Adivinhação
O programa "pensa" em um número fixo (ex: 7). O usuário tenta adivinhar. O programa continua pedindo novos palpites até que o usuário acerte o número (Dica: Use `while`).

---

## 💡 Dica da Aula: O perigoso Loop Infinito!
Sempre certifique-se de que a condição do loop em algum momento se torne falsa. Caso contrário, seu programa travará consumindo processamento infinito!
