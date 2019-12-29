# Operadores

Os operadores são usados para cálculos, comparações e atribuições.

> Cálculos = cálculos matemáticos

> Comparações = saber se algo é maior ou menor; se é igual ou diferente; etc.

> Atribuições = quando você dá valor à uma variável, veja mais em [Variáveis](./Variaveis.md)

## Principais operadores

Alguns operadores são mais usados que outros, como nós estamos aprendendo o básico, vamos explicar somente alguns aqui.

### Comparações

```javascript
a > b < c
a >= b <= c
```

### Cálculos

```javascript
a + b - c // Somar e subtrair

a * b / c // Multiplicar e dividir
```

### Verificar igualdade

Para verificar igualdade temos duas formas.

Uma simples, que compara apenas os valores.

```javascript
a == b // Se ambos são iguais ou parecidos.

a != b // Se ambos são 
```

Uma mais estrita.

> Estrita quer dizer que precisam ser EXATAMENTE iguais.

```javascript
a === b // Se ambos são EXATAMENTE IGUAIS

a !== b // Se ambos são diferentes
```

Explicando melhor a diferença:

```javascript
// Essas condições retornam TRUE
'' == false
0 == false

// Essas condições retornam FALSE
'' === false
'teste' === true
```

### Truthy e Falsy

- Truthy significa que o valor passaria num if como true
- Falsy significa que não passaria no if

**Exemplos de truthy:**

```javascript
const qtdLaranjas = 4; // truthy
const qtdUvas = 0; // falsy
const nome = 'Juliana'; // truthy
const strVazia = ''; // falsy
const arr = []; // truthy
const obj = {} // truthy

// --- Outros falsys

- null
- undefined
- ''
- 0

// --- Exemplos

if (nome) {
  // Truthy vai passar e chegar aqui
  console.log('Você tem um nome');
}

if (qtdLaranjas) {
  // Passou no if
}

if (qtdUvas) {
  // REPROVOU no if
} else {
  // Chegou aqui!
}
```

### STRICT

> Strict = estrito.

Estrito significa que o tipo da variável deve ser exatamente igual para ser `true`.

Ou seja:

```javascript
// Normal
if (0 == '0') true;

// Strict
if (0 === '0') false;
if (0 !== '0') true;
```

### Negação

O operador `!` transforma um valor em boolean, e retorna o contrário dele.

> Quando você ver dois `!!` significa que apenas queremos tranformar um parâmetro em boolean, sem alterar a propriedade "truthy" ou "falsy" dele.

> IMPORTANTE: A negação primeiramente transforma o valor em `true` ou `false` baseado no seu "valor truthy ou falsy" explicado acima.

```javascript
let numero = 10;

!numero === false
!!numero === true
```


