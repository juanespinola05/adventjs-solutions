# Reto día #14

## 🎄En busca del reno perdido

### 🟨 Normal

### En el pueblo de Santa Claus han ido a pasear a los renos y se les ha escapado uno. ¡Madre mía! Ahora a buscarlo. 😿

```js
export default function missingReindeer(ids) {
  // ¡No olvides compartir tu solución en redes!
  const sorted = ids.sort((a,b) => a > b)
  if(sorted[0] !== 0) return 0
  for(let i = 0; i < sorted.length; i++) {
    if(!(sorted[i + 1] - 1 === sorted[i])) {
      return sorted[i] + 1
    }
  }
  return sorted.length
}

```

- [Link al reto 14](https://adventjs.dev/challenges/14)
- [Link al reto anterior](./reto13.md)
- [Link al siguiente reto](./reto15.md)
