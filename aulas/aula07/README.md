# Aula 7 — Funções ⚙️

## 🎯 Conceito de Função
Uma **Função** é um bloco de código que executa uma tarefa específica. Elas são blocos independentes e reutilizáveis, organizando melhor o código principal (`main`).

---

## 🏛️ Criação de Funções
Uma função tem:
1.  **Tipo de Retorno:** O valor que ela "devolve" ao programa (ex: `int`, `float`, `void`).
2.  **Parâmetros (Entrada):** Os valores que ela recebe para trabalhar.
3.  **Bloco de Código:** O que ela faz.

```c
int somar(int a, int b) { // Os parâmetros a e b são as entradas.
    int res = a + b;
    return res; // Devolve o resultado de soma.
}
```

---

## 📜 Chamada de Função
Dentro do `main`, você chama a função pelo nome e passa os valores reais.
```c
int main() {
    int resultado = somar(10, 5); // Chama a função somar
    printf("O resultado é %d", resultado); // 15
    return 0;
}
```

---

## 🏋️ Exercícios Práticos
### 1. Função de Soma
Crie uma função que receba dois números reais (`float`) e retorne a soma deles. Chame essa função no `main` passando valores que o usuário digitar.

### 2. Conversor de Graus
Crie uma função chamada `celsiusParaFahrenheit` que receba uma temperatura em Celsius (`float`) e retorne a temperatura em Fahrenheit. Use a fórmula: `F = (C * 9/5) + 32`.

### 3. Função Par/Ímpar
Crie uma função chamada `ehPar` que receba um número inteiro e retorne `1` se ele for par ou `0` se ele for ímpar. Use um `if` dentro dessa função para decidir o retorno.

---

## 💡 Dica da Aula: Organização
Declare suas funções ANTES da função `main`. Assim, quando o compilador chegar no `main`, ele já saberá o que é cada função.
