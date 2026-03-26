# Aula 3 — Bibliotecas, Operadores e Switch-Case 📚🔀

## 📦 O que são Bibliotecas Iniciais (Includes)?
No C/C++, usamos `#include` no início do arquivo para trazer "caixas de ferramentas" prontas para usar.
*   **`<iostream>`**: Biblioteca principal de fluxos de Entrada e Saída (Input/Output Stream), base fortíssima do C++.
*   **`<stdio.h>`**: (Standard Input/Output) Traz o `printf` (para saída) e o `scanf` (para entrada) no C.
*   **`<stdlib.h>`**: (Standard Library) Permite usar funções úteis do sistema operativo.
*   **`<locale.h>`**: Configura idioma e região (localização). Excelente para problemas de acentuação!

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

**Solução 2: No Terminal do CMD / PowerShell**
Antes de compilar, digite: `chcp 65001`

---

## ➕ Operadores Aritméticos
Fazem a matemática funcionar no C:
*   `+` (Adição)
*   `-` (Subtração)
*   `*` (Multiplicação)
*   `/` (Divisão)
*   `%` (Resto da divisão, o módulo. Ex: `10 % 3` resulta em `1`, pois sobra 1).

---

## ⚖️ Operadores Relacionais (Comparações)
Verificam relações entre variáveis. O resultado é Verdadeiro ou Falso (usado em Ifs).
*   `>` (Maior que) | `<` (Menor que)
*   `>=` (Maior ou igual) | `<=` (Menor ou igual)
*   `==` (Igual a) - **Atenção:** `= ` é atribuição. `==` é comparação!
*   `!=` (Diferente de)

---

## 🧮 Operadores Lógicos (E, OU, NÃO)
Juntam múltiplas comparações em uma só.

### 1. Operador E (`&&`) - TUDO tem que ser verdade
```c
if (nota >= 7.0 && faltas < 10) {
    printf("Aprovado!\n");
}
```

### 2. Operador OU (`||`) - BASTA UMA ser verdade
```c
if (idade >= 65 || idade <= 12) {
    printf("Entrada gratuita!\n");
}
```

### 3. Operador NÃO (`!`) - Inverte a lógica
```c
if (!vip) {
    printf("Fica na fila normal.\n");
}
```

---

## 🔀 Estrutura `switch-case`
Excelente para criar **MENUS**! Substitui aquela imensa cadeia de vários `else if` quando comparamos **valores exatos** inteiros ou letras (`char`).

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
    default:
        // O default executa se não for nenhum dos cases listados
        printf("Opcao invalida!\n");
        break;
}
```

---

## 🚀 Exercício Percorrido (Construção Tática em Aula)
**Cenário Prático (Tudo junto!):** Criação do "Mercadinho Tech".
1. Mostrar opções de produtos e receber a **Opção** escolhida pelo cliente (Variáveis, Scanf, Printf).
2. Definir o **Preço** do produto baseado na escolha (Usando o `Switch-Case`). Se a opção for inválida, avisar e fechar.
3. Pedir quanto de **Dinheiro vivo** o cliente tem na carteira.
4. Mostrar Compra Aprovada ou Compra Recusada avaliando e calculando saldos e troco. Cobre Operadores Aritméticos, Relacionais e Lógicos num `If/Else`.

*(Construiremos este passo a passo juntos na IDE!)*
