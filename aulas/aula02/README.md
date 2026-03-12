# Aula 2 — Variáveis e Entrada de Dados 🏗️

## 🎯 Estrutura Básica de um Programa em C
Todo programa em C geralmente contém uma biblioteca no topo e uma função principal `main`.
```c
#include <stdio.h> // Biblioteca padrão de entrada e saída

int main() {
    // Código aqui
    return 0; // O programa terminou com sucesso
}
```

---

## 🏛️ Tipos de Variáveis
As variáveis em C são usadas para armazenar dados na memória do computador. Temos três tipos fundamentais:
*   **`int`**: Armazena números inteiros (ex: 1, -5, 100).
*   **`float`**: Armazena números de ponto flutuente, conhecidos como reais (ex: 3.14, -2.5, 10.0).
*   **`char`**: Armazena um único caractere (ex: 'A', '7', '@').

---

## 📜 Declaração de Variáveis
Sempre devemos declarar o tipo da variável antes de usá-la.
```c
int idade;
float altura;
char inicial;
```

---

## 📥 Entrada e Saída de Dados
### `printf`: Saída (Mostrar na tela)
Exibe mensagens e valores de variáveis.
```c
printf("Olá, mundo!");
printf("A idade é %d", idade); // %d é o formato para int
```

### `scanf`: Entrada (Ler do teclado)
Lê o que o usuário digita.
```c
scanf("%d", &idade); // & indica o endereço da variável
scanf("%f", &altura); // %f é o formato para float
```

---

## 🏋️ Exercícios Práticos
### 1. Ler Nome e Idade
Crie um programa que peça o primeiro nome do usuário e sua idade, exibindo uma mensagem de boas-vindas: "Olá [NOME], você tem [IDADE] anos!".

### 2. Idade no Futuro
Peça a idade atual ao usuário. Calcule e mostre quantos anos ele terá daqui a 10 anos.

### 3. Conversor de Medidas
Crie um algoritmo que leia um valor em metros e o converta para centímetros (Dica: 1 metro = 100 centímetros).

---

## 💡 Dica da Aula: Tabela de Formatos
*   `%d` ou `%i`: Inteiro (`int`).
*   `%f`: Real (`float`).
*   `%c`: Caractere (`char`).
*   `%s`: Texto (Cadeia de caracteres ou strings - veremos depois).
