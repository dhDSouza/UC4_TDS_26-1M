# Aula 1 – Revisão de JavaScript para Início de Orientação a Objetos em TypeScript 🚀

**Objetivo da aula:**
Relembrar os conceitos fundamentais de JavaScript que serão essenciais para OOP em TypeScript.

---

## 1️⃣ O que é JavaScript? 📝

* Linguagem **interpretada**, **dinâmica** e **orientada a objetos**.
* Pode rodar **no navegador** ou **no servidor** com Node.js.
* Padronização pelo **ECMAScript**.

💡 **Dica:** JS é a linguagem, Node é o ambiente que permite rodar JS fora do navegador.

---

## 2️⃣ Variáveis e Constantes 💾

```javascript
let idade = 25; // variável que pode mudar
const nome = "Daniel"; // constante, não pode mudar
```

* `let` = variável mutável
* `const` = constante imutável
* `var` = antigo, evitar
* Tipos: `number`, `string`, `boolean`, `null`, `undefined`, `object`, `array`

---

## 3️⃣ Estruturas Condicionais 🔀

### if / else

```javascript
const nota = 7;
if (nota >= 7) {
  console.log("Aprovado!");
} else if (nota >= 5) {
  console.log("Recuperação");
} else {
  console.log("Reprovado");
}
```

### Operador ternário

```javascript
const resultado = nota >= 7 ? "Aprovado" : "Reprovado";
console.log(resultado);
```

### switch / case

```javascript
const dia = 3;

switch(dia) {
  case 1:
    console.log("Domingo");
    break;
  case 2:
    console.log("Segunda");
    break;
  case 3:
    console.log("Terça");
    break;
  default:
    console.log("Outro dia");
}
```

---

## 4️⃣ Estruturas de Repetição 🔄

### for

```javascript
for (let i = 0; i < 5; i++) console.log(i);
```

### while

```javascript
let j = 0;
while (j < 5) {
  console.log(j);
  j++;
}
```

### for...of (arrays)

```javascript
const frutas = ["maçã", "banana", "laranja"];
for (const fruta of frutas) console.log(fruta);
```

### for...in (objetos ou arrays)

```javascript
const pessoa = { nome: "Daniel", idade: 25 };
for (const chave in pessoa) {
  console.log(`${chave}: ${pessoa[chave]}`);
}
```

### forEach (arrays)

```javascript
const numeros = [1, 2, 3, 4, 5];
numeros.forEach((num) => console.log(num));
```

---

## 5️⃣ Funções 🛠️

### Tradicional

```javascript
function soma(a, b) {
  return a + b;
}
```

### Arrow function

```javascript
const subtrai = (a, b) => a - b;
```

---

## 6️⃣ Node.js e Comandos de Terminal 💻

* `node arquivo.js` → Executa script JS
* `console.log()` → Mostra saída no terminal

---

## 7️⃣ Entrada de dados do usuário 📝

### prompt (navegador)

```javascript
const nome = prompt("Qual seu nome?");
console.log(`Olá, ${nome}!`);
```

### readline-sync (Node.js) ⚡

```javascript
const readlineSync = require('readline-sync');
const name = readlineSync.question('What is your name? ');
console.log(`Hello, ${name}!`);
```

---

## 8️⃣ O que é NPM? 📦

* **Node Package Manager**, gerenciador de pacotes do Node.
* Permite instalar bibliotecas externas:

```bash
npm init -y
npm install readline-sync
```

* `readline` não precisa de NPM, mas outras libs sim.

---

## 9️⃣ Exercícios de Revisão 🏋️‍♂️ (15 exercícios)

### Variáveis, operadores e entrada/saída

1. Peça o nome e idade do usuário e mostre uma mensagem personalizada.
2. Solicite dois números e mostre a soma, subtração, multiplicação e divisão.
3. Peça uma nota e exiba “Aprovado” ou “Reprovado” usando operador ternário.
4. Verifique se um número é par ou ímpar usando `if/else`.

### Estruturas condicionais

5. Peça o dia da semana (1-7) e use `switch` para mostrar o nome do dia.
6. Crie um mini-cardápio e use `switch` para mostrar o preço do item escolhido.

### Loops

7. Crie um array de 5 números e calcule a soma usando `for`.
8. Faça um loop `while` que exiba números de 1 a 10.
9. Use `for...of` para imprimir todos os elementos de um array de frutas.
10. Use `forEach` para imprimir todos os elementos de um array de cores.
11. Crie um objeto `pessoa` com `nome` e `idade` e use `for...in` para imprimir cada propriedade.
12. Faça um loop que exiba todos os números pares de 0 a 20.

### Funções

13. Crie uma função tradicional que receba 2 números e retorne o maior.
14. Crie uma arrow function que receba um array e retorne a soma de todos os elementos.
15. Crie uma função que peça ao usuário seu nome e idade (usando readline) e exiba uma saudação personalizada.
