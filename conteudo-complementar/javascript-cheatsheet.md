# 📋 JavaScript Cheatsheet

## Variáveis
var x = 1;      # escopo global (evitar)
let y = 2;      # escopo de bloco
const z = 3;    # constante

## Tipos
string, number, boolean, null, undefined, object, array

## Strings
s.length
s.toUpperCase()
s.toLowerCase()
s.includes("texto")
s.split(",")
`Olá ${nome}`   # template literal

## Arrays
arr.push(val)
arr.pop()
arr.shift()
arr.unshift(val)
arr.map(x => x * 2)
arr.filter(x => x > 0)
arr.reduce((acc, x) => acc + x, 0)
arr.find(x => x > 2)
arr.forEach(x => console.log(x))

## Objetos
const obj = { chave: "valor" }
obj.chave
obj["chave"]
const { chave } = obj   # destructuring

## Controle de fluxo
if (x > 0) {}
for (let i = 0; i < 10; i++) {}
while (x > 0) {}
x > 0 ? "sim" : "não"   # ternário

## Funções
function soma(a, b) { return a + b }
const soma = (a, b) => a + b

## DOM
document.querySelector(".classe")
document.getElementById("id")
elemento.innerHTML = "texto"
elemento.addEventListener("click", fn)

## Fetch
fetch("url")
  .then(res => res.json())
  .then(data => console.log(data))
  .catch(err => console.error(err))

## Assincronismo (Promises e Async/Await)
async function buscar() {
  try {
    const res = await fetch("url");
    const data = await res.json();
  } catch (err) {
    console.log(err);
  }
}

## Módulos e Operadores
import { modulo } from "./arquivo.js";
export const valor = 10;
const copiaArr = [...arr];       # spread operator (cópia de array)
const novoObj = { ...obj, a: 1 } # spread em objetos