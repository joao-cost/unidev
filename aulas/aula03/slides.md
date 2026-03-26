# Aula 3 — Bibliotecas, Operadores Lógicos e Switch-Case 📚🔀

## 📦 O que são Bibliotecas Iniciais (Includes)?
No C, usamos `#include` no início do arquivo para trazer "caixas de ferramentas" prontas para usar.
*   **`<stdio.h>`**: (Standard Input/Output) Traz o `printf` (para saída) e o `scanf` (para entrada).
*   **`<stdlib.h>`**: (Standard Library) Permite usar funções úteis do sistema operativo (ex: limpar a tela).
*   **`<locale.h>`**: Configura idioma e região (localização). Excelente para consertar problemas de acentuação!

---

## 🌎 O Problema do UTF-8 e Acentuação no Windows
O terminal (prompt de comando) do Windows muitas vezes não entende acentos como "ç", "á" e exibe caracteres estranhos (`Æ`, `¢`).
**Solução 1: Com `#include <locale.h>` no código**
```c
#include <stdio.h>
#include <locale.h> // 1. Inclui a biblioteca

int main() {
    // 2. Configura o C para usar o idioma do computador (acentos funcionam!)
    setlocale(LC_ALL, "Portuguese"); 
    
    printf("Olá, mundo! Acentuação ativada.\n");
    return 0;
}
```

**Solução 2: No Terminal do Windows (CMD / PowerShell)**
Antes de compilar e rodar seu programa, digite no terminal:
`chcp 65001`
*(Isso muda forçadamente a codificação do console para UTF-8).*

---

## 🧮 Operadores Lógicos (E, OU, NÃO)
Quando apenas um `if` normal não é suficiente, nós usamos operadores lógicos para juntar múltiplas condições.

### 1. Operador E (`&&`) - TUDO tem que ser verdade
A condição só será aceita se **ambas as partes** forem verdadeiras.
```c
// Queremos aprovar quem tem nota >= 7 E poucas faltas.
if (nota >= 7.0 && faltas < 10) {
    printf("Aprovado!\n");
}
```

### 2. Operador OU (`||`) - BASTA UMA ser verdade
A condição será aceita se **pelo menos uma das partes** for verdadeira.
```c
// Entrada grátis para idosos OU crianças.
if (idade >= 65 || idade <= 12) {
    printf("Entrada gratuita!\n");
}
```

### 3. Operador NÃO (`!`) - Inverte a lógica
Executa quando algo é **falso** ou igual a **zero**.
```c
// Se NÃO for Vip (ou seja, se vip for igual a 0)
if (!vip) {
    printf("Fica na fila normal.\n");
}
```

---

## 🔀 Estrutura `switch-case`
Excelente para criar **MENUS**! Substitui aquela imensa cadeia de vários `else if` quando estamos comparando **valores exatos e inteiros** (como `1`, `2`, `'A'`, `'B'`).

```c
int opcao;
printf("1-Saldo | 2-Saque | 3-Sair\nEscolha: ");
scanf("%d", &opcao);

switch (opcao) {
    case 1:
        printf("Seu saldo: R$ 100,00\n");
        break; // IMPORTANTE: O break sai do bloco switch!
    case 2:
        printf("Saque realizado.\n");
        break;
    case 3:
        printf("Saindo...\n");
        break;
    default:
        // O default executa se você não digitar nenhuma das opções acima
        printf("Opcao invalida!\n");
        break;
}
```
