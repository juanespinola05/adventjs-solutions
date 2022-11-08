# Reto día #13

## 🎄Envuelve regalos con asteriscos

### 🟩 Fácil

### Estamos a fuego envolviendo regalos... ¡pero necesitamos automatizar esto antes de que los elfos decidan ponerse en huelga! ¡Salva la Navidad (otra vez)!

```js
export default function wrapGifts(gifts) {
  // ¡No olvides compartir tu solución en redes!
  const wrappedGifts = gifts.reduce((acc, curr, i, array) => {
    if(i === 0) acc.push("*".repeat(curr.length + 2))
    acc.push("*" + curr + "*")
    if(i === array.length - 1) acc.push("*".repeat(curr.length + 2))
    return acc
  }, [])
  return wrappedGifts
}
```

- [Link al reto 13](https://adventjs.dev/challenges/13)
- [Link al reto anterior](./reto12.md)
- [Link al siguiente reto](./reto14.md)
