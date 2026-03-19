# Aula 2 — Slides de Variáveis e Dados 🏗️

## 🎯 Estrutura Básica de um Programa C
```c
#include <stdio.h>
int main() {
    return 0;
}
```

---

## 🏛️ Variáveis: Tipos e Declaração
*   **`int`**: Inteiros. Ex: `int idade;`
*   **`float`**: Reais. Ex: `float altura;`
*   **`char`**: Caracteres. Ex: `char letra;`

---

## 📥/📤 Entrada e Saída (Resumo Rápido)
*   **`printf` (`%d`, `%f`, `%c`)**: Mostra informação na tela.
*   **`scanf`**: Lê dado digitado no teclado.

**Exemplo Prático:**
```c
int idade;
printf("Digite sua idade: ");
scanf("%d", &idade);
```

---

## 🔀 Estruturas de Condição (IF / ELSE IF / ELSE)
Servem para o programa tomar decisões baseadas em condições matemáticas ou lógicas.

### 1. `if` (Se)
Executa se a condição for verdadeira.
```c
if (idade >= 18) {
    printf("Pode entrar na festa!\n");
}
```

### 2. `else` (Senão)
Alternativa caso o `if` seja falso.
```c
if (idade >= 18) {
    printf("Maior de idade.\n");
} else {
    printf("Menor de idade.\n");
}
```

### 3. `else if` (Senão, se)
Testa múltiplas condições em sequência.
```c
if (nota >= 7.0) {
    printf("Aprovado!\n");
} else if (nota >= 5.0) {
    printf("Recuperacao.\n");
} else {
    printf("Reprovado.\n");
}
```
