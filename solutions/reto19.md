# Reto día #19

## 🎄 ¿Qué deberíamos aprender en Platzi?

### 🟨 Normal

### ¡Hay un montón de cursos en Platzi! Queremos hacer dos cursos y nuestro tiempo es limitado. ¡Vamos a crear una función para elegir los dos mejores cursos a hacer según nuestro tiempo!

```js
export default function learn(time, courses) {
  let bestOption = { total: 0, pair: []}
	for(let i = 0; i < courses.length; i++) {
    for(let j = i + 1; j < courses.length; j++) {
      const total = courses[i] + courses[j]
      if(total <= time && total > bestOption.total) {
        bestOption = {total, pair: [i, j]}
      }
    }
  }
  return bestOption.pair.length ? bestOption.pair : null
}

```

- [Link al reto 19](https://adventjs.dev/challenges/19)
- [Link al reto anterior](./reto18.md)
- [Link al siguiente reto](./reto20.md)
