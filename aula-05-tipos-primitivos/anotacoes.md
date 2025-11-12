# Aula 5 - Tipos primitivos

Assim como no JavaScript, os tipos primitivos são os mais básicos e mais utilizados

São aqueles que você normalmente obtém usando o operador `typeof`

Existem três mais utilizados

- **boolean:** os valores que equivalem a **true** ou **false**

```ts
let maiorIdade: boolean = true
```

- **number:** como o JavaScript não diferencia inteiros e pontos flutuantes, tudo é apenas considerado como number também no TypeScript

```ts
let idade: number = 23
```

- **string:** valores de texto, como "Hello, world!"

```ts
let nome: string = 'Pedro Otávio'
```

Além disso, temos também o **Array**, que representa as listas de dados

- A sintaxe básica para especificar um array é utilizando o tipo dos seus elementos. Por exemplo, `string[]` ou `number[]`

```ts
let inteiros: number[] = [-2, -1, 0, 1, 2]
```

```ts
// Tipos genéricos
Array<number> = [2, 4, 6, 8]
```

- Idealmente, usamos arrays como sendo uma lista onde todos os elementos têm o **mesmo tipo**, mas esse comportamento também pode ser evitado