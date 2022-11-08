# Reto día #12

## 🎄La ruta perfecta para dejar los regalos

### 🟥 Difícil

### En el taller de Santa ya están preparándolo todo para poder hacer la ruta perfecta para dejar los regalos. El problema es que hay unos obstáculos en el camino que debemos sortear...

```js
export default function getMinJump(obstacles) {
  // ¡No olvides compartir tu solución en redes!
  if(!obstacles.length) return 1
  const maxPositions = Math.max(...obstacles)
  let min = 1
  for(let i = 2; i <= maxPositions; i++) {
    for(let j = 1; j < maxPositions; j++) {
      if(obstacles.includes(i*j)) {
        min = null
        break
      }
      min = i
    }
    if(min) return i
  }
  
  return min
}
```

- [Link al reto 12](https://adventjs.dev/challenges/12)
- [Link al reto anterior](./reto11.md)
- [Link al siguiente reto](./reto13.md)
