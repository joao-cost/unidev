# Aula 6 — Slides de Vetores (Arrays) 📊

## 🎯 O que é um Vetor?
Varíavel que armazena múltiplos valores do mesmo tipo.
Como uma lista de gavetas numeradas.

## 🏛️ Declaração e Acesso
`int idades[5];`
Índices começam em **0** e vão até o **tamanho - 1**.

---

## 📜 Percorrendo um Vetor
Usamos o loop `for` para acessar cada posição de forma automática.

```c
for (int i = 0; i < 5; i++) {
    printf("%d", idades[i]);
}
```
