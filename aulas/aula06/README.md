# Aula 6 — Vetores (Arrays) 📊

## 🎯 Conceito de Vetor
Um **Vetor** é uma variável especial que pode armazenar múltiplos valores do mesmo tipo. Imagine uma lista de gavetas, onde cada gaveta tem um índice (começando em 0).

---

## 🏛️ Declaração e Acesso
Sempre declaramos o tipo e o tamanho do vetor entre colchetes (`[ ]`).
```c
int idades[5]; // Reserva espaço para 5 números inteiros
```

### Acesso por Índice
A primeira "gaveta" é sempre o índice **0**. A última é o **tamanho - 1**.
```c
idades[0] = 18; // Primeira posição
idades[4] = 25; // Última posição (se o tamanho for 5)
```

---

## 📜 Percorrendo um Vetor com Loop
Muitas vezes, usamos o `for` para passar por cada posição do vetor.
```c
for (int i = 0; i < 5; i++) {
    printf("A idade na posição %d é %d\n", i, idades[i]);
}
```

---

## 🏋️ Exercícios Práticos
### 1. Lista de Compras (Exemplo: Preços)
Crie um programa que peça ao usuário os preços de 10 produtos e os armazene em um vetor do tipo `float`. No final, mostre todos os preços lidos.

### 2. Média da Turma
Armazene 5 notas de alunos em um vetor. No final, calcule a média da turma toda.

### 3. Maior do Vetor
Crie um programa que leia 10 números inteiros, salve em um vetor e informe qual é o maior número dentro dele.

---

## 💡 Dica da Aula: O índice vai apenas até o final!
Cuidado ao tentar acessar um índice que não existe. Se o vetor tem tamanho 5, os índices são 0, 1, 2, 3 e 4. Tentar acessar o índice 5 causará erro ou trará lixo de memória!
