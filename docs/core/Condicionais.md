# Condicionais

## Condições

As condições no javascript são muito importantes.

**Observações**

> Dentro do if, temos uma CONDIÇÃO

> Dentro de um ternário, temos uma CONDIÇÃO

> Dentro do return, podemos ter um ternário, ou seja, uma condição

Para mais detalhes, consulte os [Operadores](./Operadores.md)

```javascript
const idade = 18;

idade > 10 === true
idade * 2 < 20 === false
!!idade === true
!idade === false
```


## IF e ELSE

O if serve para executar um bloco de códigos se o "teste" for verdadeiro.

> `{ bloco de código é um código que fica dentro de chaves }`

```javascript
var nome = 'Patrik';
var idade = 23;

if (idade >= 18) {
  console.log('Sou de maior');
}

if (nome === 'Robson') {
  console.log('Olá Robson');
}
```

### ELSE

O else é executado apenas se a condição do if for `false`.

```javascript

var idade = 8 * 2;

if (idade > 17) {
  console.log('Você é de maior');
} else {
  console.log('Você é criança');
}

```
