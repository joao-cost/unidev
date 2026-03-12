# Aula 3 — Operadores e Cálculos ➕

## 🎯 Operadores Matemáticos básicos em C
Os operadores matemáticos permitem realizar cálculos e transformações de dados. Em C, temos os seguintes:
*   `+`: Soma.
*   `-`: Subtração.
*   `*`: Multiplicação.
*   `/`: Divisão.
*   `%`: Módulo (resto da divisão inteira).

### Exemplo: Cálculo Simples
```c
#include <stdio.h>

int main() {
    int a = 10, b = 3;
    int soma = a + b;     // 13
    int resto = a % b;   // 1 (porque 10 / 3 dá 3 e resta 1)
    
    printf("Soma: %d, Resto: %d", soma, resto);
    return 0;
}
```

---

## 🏛️ Expressões Matemáticas
Lembre-se da ordem das operações em matemática:
1.  Parênteses `()`.
2.  Multiplicação e Divisão `*` e `/`.
3.  Soma e Subtração `+` e `-`.

```c
int res = 10 + 2 * 3; // O resultado é 16, pois 2 * 3 vem primeiro.
```

---

## 🏋️ Exercícios Práticos
### 1. Calculadora Simples
Crie um programa que leia dois números reais (`float`) e exiba os resultados de: soma, subtração, multiplicação e divisão.

### 2. Cálculo de Média
Um aluno fez três provas durante o semestre. Peça as notas delas ao usuário e exiba a média final (Dica: media = (n1 + n2 + n3) / 3.0).

### 3. Cálculo de IMC
Crie um programa que peça ao usuário seu peso (kg) e sua altura (m). Calcule o seu Índice de Massa Corporal (IMC) usando a fórmula: `IMC = peso / (altura * altura)`. Exiba o resultado com duas casas decimais using `%.2f` no printf.

---

## 💡 Dica da Aula: O perigo da Divisão Inteira
Se você dividir dois números inteiros (`int / int`), o resultado será sempre um inteiro truncado (ex: 5 / 2 = 2, não 2.5). Se quiser a casa decimal, declare pelo menos uma das variáveis como `float`.
