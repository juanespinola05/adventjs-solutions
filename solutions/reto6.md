# Reto día #6

## 🎄Rematando los exámenes finales

### 🟨 Normal

### Buffff! Ya huelo las vacaciones pero todavía falta terminar los exámenes finales. ¡Y toca un poco de matemáticas! 😱 ¡Ayúdame!

```js
export default function sumPairs(numbers, result) {
  // ¡Y no olvides compartir tu solución en redes!
  let pair = [];
  for (let i = 0; i < numbers.length; i++) {
    for (let j = i + 1; j < numbers.length; j++) {
      if (numbers[i] + numbers[j] === result) {
        pair.push(numbers[i], numbers[j]);
        return pair;
      }
    }
  }
  return null;
}
```

- [Link al reto 6](https://adventjs.dev/challenges/06)
- [Link al reto anterior](./reto5.md)
- [Link al siguiente reto](./reto7.md)
