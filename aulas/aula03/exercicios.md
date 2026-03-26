# 🏋️ Exercícios da Aula 3

## Atividade 1 — Verificador de Ano Bissexto
**(Engloba Aula 2 + Operadores Lógicos)**

**Enunciado:**
Um ano é considerado bissexto se for divisível por 400 **OU** se for divisível por 4 **E** não for divisível por 100.
Escreva um programa que peça ao usuário um ano (ex: 2024) e exiba na tela se ele é "Bissexto" ou "Não Bissexto". Utilize os operadores lógicos `&&` e `||` dentro de um único `if`.

---

## Atividade 2 — Acesso ao Sistema
**(Engloba Variáveis + Operadores Lógicos)**

**Enunciado:**
Crie um programa que simule a entrada num sistema restrito. 
Peça ao usuário para digitar uma "senha" numérica e o seu "ano de nascimento".
O acesso só é **Concedido** se a senha estiver correta (ex: senha igual a `12345`) **E** o usuário for maior de idade (calculando `ano_atual - ano_nascimento >= 18`). Caso contrário, o acesso deve ser **Negado**.

---

## Atividade 3 — Menu de Calculadora Simples
**(Foco em Switch-Case)**

**Enunciado:**
Crie um programa que receba dois números lidos com `%f` (float) fornecidos pelo usuário. Em seguida, mostre um menu:
1. Somar
2. Subtrair
3. Multiplicar
4. Dividir

Peça para ele digitar a opção desejada. Use a estrutura `switch / case` para verificar a `opcao` inserida, realizar o cálculo escolhido e mostrar o resultado. Lembre-se, caso ele escolha divisão (Opção 4), verifique se o segundo número é zero antes de dividir (você pode usar um `if/else` dentro do `case`!). Se a opção digitada for diferente de 1 a 4, avise através do caso `default` que a opção foi inválida.

---

## Atividade 4 — Classificação de Produtos
**(Foco em Switch-Case)**

**Enunciado:**
Leia do usuário o código de um determinado produto (número inteiro) e informe a sua categoria segundo a tabela:
- Código 1: Alimento não-perecível
- Código 2, 3 ou 4: Alimento perecível
- Código 5 ou 6: Vestuário
- Código 7: Higiene pessoal
- Valores fora dessa tabela: Categoria Inválida

Dica: No `switch`, você pode encadear `case` numéricos vazios para que várias escolhas recebam exatamente a mesma impressão, por exemplo:
```c
case 2:
case 3:
case 4:
    printf("Perecivel\n");
    break;
```

---

**Dica Geral para a Aula:** Tente implementar em todos os exercícios o seu novo `#include <locale.h>` acompanhado do comando `setlocale(LC_ALL, "Portuguese");` logo no início da sua função `main()`. Assim, teremos tranquilidade garantida com os acentos no Windows!
