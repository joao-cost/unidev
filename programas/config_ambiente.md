# Configurando seu Ambiente de Programação 💻

Para programar em C, precisamos de um **Compilador** (que traduz seu código para a linguagem do computador) e um **Editor** (onde você escreve o código). O **Dev-C++ Portable** que vamos usar já vem com os dois!

---

## 📥 Download do Programa
Para facilitar, utilize a versão portable que não precisa de instalação:

👉 **[Baixar Dev-C++ 5.11 Portable](https://unidev-unemat.s3.us-east-005.backblazeb2.com/programas_unidev/Dev-Cpp+5.11+TDM-GCC+x64+4.9.2+Portable.7z)**

---

## 🛠️ Tutorial de Instalação e Uso

### 1. Extração
Como o arquivo está no formato `.7z`, você precisará de um programa como o **7-Zip** ou **WinRAR** para extrair.
1. Clique com o botão direito no arquivo baixado.
2. Escolha "Extrair para..." ou "Extrair aqui".
3. Abra a pasta extraída e procure pelo ícone do **devcpp.exe**.

### 2. Criando seu Primeiro Arquivo
1. Abra o Dev-C++.
2. Vá em **Arquivo (File)** -> **Novo (New)** -> **Arquivo Fonte (Source File)**.
3. Ou use o atalho: `Ctrl + N`.

### 3. Escrevendo o Código
Digite o código abaixo para testar:
```c
#include <stdio.h>

int main() {
    printf("Ambiente configurado com sucesso!\n");
    return 0;
}
```

### 4. Salvando o Arquivo
1. Vá em **Arquivo** -> **Salvar**.
2. **IMPORTANTE:** Salve sempre com a extensão **.c** (ex: `teste.c`). Por padrão, ele pode tentar salvar como `.cpp`, certifique-se de mudar para **C source files (*.c)** na caixa de tipo.

### 5. Compilar e Rodar
Existem três botões coloridos no topo ou você pode usar as teclas de atalho:
*   **F9 (Compilar):** Verifica se há erros no seu código.
*   **F10 (Executar):** Abre o terminal e mostra o resultado.
*   **F11 (Compilar e Executar):** Faz os dois de uma vez (O mais usado!).

---

## ⚠️ Dicas e Solução de Problemas
*   **Tela fecha rápido:** Se o programa rodar e a tela preta sumir instantaneamente, adicione `getchar();` antes do `return 0;`.
*   **Erros em vermelho:** Se aparecerem linhas vermelhas na parte de baixo após apertar F9, leia a mensagem! Ela diz exatamente em qual linha você esqueceu um `;` ou cometeu um erro de digitação.
*   **Portabilidade:** Como esta versão é portable, você pode colocar a pasta em um pendrive e programar em qualquer computador da faculdade sem precisar instalar nada!
