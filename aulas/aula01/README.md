# Aula 1 — Introdução à Programação 🚀

## 🎯 O que é Programação?
Programação é o processo de escrever instruções para que um computador execute tarefas e resolva problemas.
Imagine dar uma receita de bolo para o computador: ele deve seguir cada passo exatamente como descrito.

## 🏛️ O que é um Algoritmo?
Um **Algoritmo** é uma sequência finita de passos bem definidos para resolver um problema.
Qualquer tarefa pode ser um algoritmo:
*   Amarrar os sapatos.
*   Fazer um café.
*   Calcular a média de um aluno.

---

## 🏗️ Estrutura de um Algoritmo
Todo algoritmo segue este ciclo básico:
1.  **Entrada:** Dados fornecidos pelo usuário ou sensores.
2.  **Processamento:** Operações matemáticas, lógicas ou transformações.
3.  **Saída:** Resultado final exibido na tela, impresso ou armazenado.

---

## 🗺️ Fluxograma
É a representação gráfica de um algoritmo. Abaixo estão os principais símbolos utilizados:

![Símbolos do Fluxograma](img/simbolos_fluxograma.png)

*   **Elipse (Início/Fim):** Indica onde o algoritmo começa e termina.
*   **Paralelogramo (Entrada/Saída):** Representa a leitura de dados ou a exibição de resultados.
*   **Retângulo (Processamento):** Indica cálculos ou atribuições de valores.
*   **Losango (Decisão):** Uma pergunta que altera o fluxo do programa (Sim ou Não).

### Exemplo: Atravessar a Rua
Veja como desenharíamos a lógica para atravessar uma rua com segurança:

![Exemplo de Fluxograma - Atravessar a Rua](img/fluxograma_rua.png)

---

## 📜 Portugol e Portugol WebStudio
O Portugol é uma "linguagem" (pseudocódigo) usada para ensinar lógica usando termos em português. Facilita o aprendizado antes de partir para a sintaxe rígida de linguagens reais.

### Onde praticar?
Recomendamos o **Portugol WebStudio**, que não precisa instalar nada!
👉 **[Acesse o Portugol WebStudio aqui](https://portugol.devpost.com.br/)** *(ou busque por Portugol WebStudio no Google)*

### Exemplo: Primeiro Algoritmo em Portugol
```portugol
programa {
  funcao inicio() {
    escreva("Olá, Desenvolvedor!")
  }
}
```

---

## 💻 Tradução para Linguagem C
Agora que entendemos a lógica, veja como o mesmo código ficaria em C:

```c
#include <stdio.h>

int main() {
    printf("Olá, Desenvolvedor!\n");
    return 0;
}
```

---

## 🏋️ Exercício da Aula
1. **Lógica no Papel:** Tente desenhar um fluxograma para o processo de "Fazer um Café". Não esqueça da decisão: "O café está doce o suficiente?".
2. **Portugol WebStudio:** Entre no site e tente fazer o código acima que escreve o "Olá".
3. **Ambiente C:** Se já configurou seu [Dev-C++](../../programas/README.md), execute seu primeiro "Olá Mundo!" em C.
