# Projeto: O Jogo da Imitação (ML e Criptografia)

Este projeto foi inspirado no trabalho de Alan Turing e no filme "O Jogo da Imitação". Ele é um site estático com duas atividades práticas desenvolvidas em JavaScript para explorar conceitos de Machine Learning e Criptografia.

## 🚀 Membros do Grupo

* [Nome do Aluno 1]
* [Nome do Aluno 2]
* [Nome do Aluno 3]

## 📂 Estrutura do Site

O projeto agora é um site unificado com navegação entre as duas atividades:

* **`index.html`**: O Desafio 2 (Jogo do Hash).
* **`ml.html`**: O Desafio 1 (Regressão ML).
* **`style.css`**: Folha de estilos compartilhada para ambas as páginas.

---

## 🔑 Desafio 2: O Jogo do Hash (A Frase Secreta) - `index.html`

Esta atividade demonstra um princípio fundamental da criptografia moderna: a natureza "mão única" (one-way) dos algoritmos de hash (SHA-256).

* **Objetivo:** O usuário não deve "quebrar" o hash, mas sim usar um sistema de dicas para **deduzir** a frase secreta que gera o hash.
* **Como Funciona:**
    1.  O computador define uma frase complexa secreta e calcula seu hash SHA-256.
    2.  O hash é exibido para o usuário.
    3.  O usuário pode solicitar até 5 dicas para ajudar a deduzir a frase.
    4.  O usuário digita sua tentativa. O script calcula o hash da tentativa e o compara com o hash alvo.
* **Tecnologia:** API nativa `SubtleCrypto` do navegador (SHA-256) e manipulação de DOM.

---

## 🤖 Desafio 1: Regressão Linear com TensorFlow.js - `ml.html`

Esta atividade demonstra um modelo de Machine Learning simples para regressão linear, executado 100% no navegador.

* **Objetivo:** Treinar um modelo para "aprender" a fórmula matemática $Y = 2X - 1$.
* **Tecnologia:** TensorFlow.js (`@tensorflow/tfjs`).
* **Como Executar:**
    1.  Abra o arquivo `ml.html` em qualquer navegador web.
    2.  Abra o Console do Desenvolvedor (F12).
    3.  Observe o log de treinamento (a "perda" ou "loss" deve diminuir a cada época).
    4.  Ao final, o console exibirá a previsão do modelo para X=10 (o resultado esperado é ~19.0).