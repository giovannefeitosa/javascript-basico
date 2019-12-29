# Loops

Vamos explicar apenas os loops principais por enquanto

## FOR

O for é um dos mais utilizados.

Exemplo mais comum (Quase não usamos mais assim).

> Use para fazer loop em um **INTERVALO DE NÚMEROS**

```javascript

const inicio = 0;
const fim = 5;

for (let i = inicio; i < fim; i++) {
  // Vai de 0 até 4
  // Porque o operador exige que i seja < que fim
}

for (let i = 0; i <= 5; i++) {
  // Vai de 0 até 5
  // Por causa do operador <=
}

```

## FOR IN e FOR OF

> Use para fazer loops em ARRAYS

```javascript
const lista = ['a', 'b', 'c', 'd'];

// --- FOR IN
// atribui o index

// index = 0 | 1 | 2 | 3
for(const index in lista) {
  console.log(index);
}

// --- FOR OF
// atribui o valor da variável
// parecido com o map

// item = 'a' | 'b' | 'c' | 'd'
for (const item of lista) {
  console.log(item);
}
```

## MAP

> Use para fazer loops em ARRAYS

O map é utilizado para transformar arrays.

```javascript
const nomes = ['Elon Musk', 'Steve Jobs', 'Ronaldo'];

// --- Transformar cada item em um número

const indexes = nomes.map(function(nome, index) {
  return index;
});

// [0, 1, 2]
console.log(indexes);

// --- Transformar cada item em letras maiúsculas

const maiusculas = nomes.map((nome, index) => {
  return nome.toUpperCase();
});

// ['ELON MUSK', 'STEVE JOBS', 'RONALDO']
console.log(maiusculas);



// --- DICA REACT

// --- Transformar em componentes REACT
return (
  <div className="Lista de nomes">
    {nomes.map((nome, index) => {
      return (
        <div key={index}>
          {index} - {nome}
        </div>
      );
    })}
  </div>
);
```
