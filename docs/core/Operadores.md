# Operadores

Os operadores são usados para cálculos, comparações e atribuições.

> Cálculos = cálculos matemáticos

> Comparações = saber se algo é maior ou menor; se é igual ou diferente; etc.

> Atribuições = quando você dá valor à uma variável, veja mais em [Variáveis](./Variaveis.md)

## Principais operadores

Alguns operadores são mais usados que outros, como nós estamos aprendendo o básico, vamos explicar somente alguns aqui.

### Comparações

```javascript
a > b
a < b
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
