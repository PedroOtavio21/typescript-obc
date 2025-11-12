# Aula 6 - Inferência de tipo

O VsCode possui uma funcionalidade bem bacana, onde mesmo que não seja explicado o que uma determinada variável ou método faz, 
a IDE é inteligente o bastante para retornar um código inferido (uma expécie de correção)

Exemplo 1:

```ts
// O seguinte código abaixo:
const spaceship = {name: "X-Wind", speed: 0}

// É interpretado da seguinte forma:
const spaceship: {
    name: string;
    speed: number;
}
```

Exemplo 2:

```ts
// A seguinte função abaixo
function accelerate(spaceship, speed){
    // ...
}

accelerate(spaceship, 50)

// Poderá ser convertida em:
function accelerate(spaceship: { name: string; speed: number }, speed: number){
    spaceship.speed = speed
}
```