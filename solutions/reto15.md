# Reto día #15

## 🎄El salto perfecto

### 🟨 Normal

### Estamos optimizando el trineo para que los saltos que da sean lo más óptimos posible. Un amigo que tiene un Tesla nos ha explicado la mejor forma. ¡A ver si sacamos una función para aseguarnos!

```js
export default function checkSledJump(heights) {
  let limit = null
  let i;
  let strict = true
  for(i = 1; i < heights.length; i++) {
    if(!(heights[i] > heights[i- 1]) || i === heights.length-1) {
      limit = heights[i - 1]
      break
    }
  }
  for(i; i < heights.length; i++) {
    if(!(heights[i] < heights[i - 1])) {
      strict = false
    }
  }
  return strict
}

```

- [Link al reto 15](https://adventjs.dev/challenges/15)
- [Link al reto anterior](./reto14.md)
