# Reto día #8

## 🎄La locura de las criptomonedas

### 🟨 Normal

### Hemos invertido en criptomonedas... Y el otro día se pusieron todos los valores en rojo. En lugar de asustarnos, vamos a ver si podemos optimizar nuevas inversiones.

```js
export default function maxProfit(prices) {
  // ¡Y no olvides compartir tu solución en redes!
  let max = -1;
  prices.reduce((acc, curr, index, array) => {
    for (let i = index; i < array.length; i++) {
      const profit = array[i] - acc;
      if (acc > array[i] || profit <= 0) continue;
      max = profit > max ? profit : max;
    }
    return array[index];
  });
  return max;
}
```

- [Link al reto 8](https://adventjs.dev/challenges/08)
- [Link al reto anterior](./reto7.md)
- [Link al siguiente reto](./reto9.md)
