# Aula 8 — Projeto Final 🏁

## 🎯 Objetivo: Sistema de Almoxarifado em C (Terminal)
O projeto final desta trilha consiste na criação de um sistema básico de controle de estoque de um almoxarifado, funcional via terminal. O sistema deve permitir as operações fundamentais de gerência.

---

## 🏛️ Funcionalidades do Projeto
O sistema deve apresentar um menu interativo com as seguintes opções:

1.  **Cadastrar Item:** Adicionar um novo produto ao estoque (Nome e Quantidade).
2.  **Listar Itens:** Mostrar todos os itens cadastrados no estoque e suas quantidades.
3.  **Editar Item:** Alterar o nome ou a quantidade de um item já cadastrado.
4.  **Deletar Item:** Remover um item do estoque do almoxarifado.
5.  **Encerrar Programa.**

---

## 📜 Conceitos Utilizados
Para construir este projeto, você usará todos os conhecimentos anteriores:
*   **Structs**: Para organizar os dados do item (ex: `struct Item { char nome[50]; int quantidade; };`).
*   **Vetores**: Para armazenar uma lista de structs (itens).
*   **Loops (`while`)**: Para manter o menu interativo rodando até o usuário sair.
*   **Switch Case / if**: Para escolher a opção do menu.
*   **Funções**: Para cada uma das funcionalidades (ex: `cadastrarItem()`, `mostrarEstoque()`, etc).

---

## 🏗️ Estrutura Sugerida
O seu programa deve seguir uma estrutura limpa:
```c
#include <stdio.h>
#include <string.h>

// 1. Definição da Struct (ex: struct Produto)
// 2. Declaração do Vetor (ex: struct Produto estoque[100]; )
// 3. Implementação das Funções (cadastrar, listar, etc)
// 4. Função Principal (main) com o Menu em loop
```

---

## 🏆 Resultado Esperado
Ao concluir o projeto final, você terá consolidado seus conhecimentos em lógica de programação e fundamentos da linguagem C, entregando um software funcional e estruturado pronto para evoluir para tecnologias mais complexas.

---

## 🚀 Próximos Passos
Após esta trilha, você estará preparado para:
- Estudar Alocação Dinâmica de Memória (Ponteiros).
- Manipulação de Arquivos e Bancos de Dados.
- Linguagens Modernas (C++, Java, Python, JavaScript).
