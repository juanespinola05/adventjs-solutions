# Reto día #10

## 🎄La máquina de cambio

### 🟥 Difícil

### De cara a las ventas navideñas, vamos a automatizar el cambio de las monedas para que no se tenga que hacer manualmente. ¡Ganaremos tiempo! Pero primero, hay que programarlo.

- [Link al reto 10](https://adventjs.dev/challenges/10)
- [Link al reto anterior](./reto9.md)

```js
export default function getCoins(change) {
  // ¡No olvides compartir tu solución en redes!
  const cents = [1, 2, 5, 10, 20, 50];
  const coins = [0, 0, 0, 0, 0, 0];
  cents.reverse().forEach((item, i) => {
    coins[i] = Math.floor(change / item);
    change -= coins[i] * item;
  });
  return coins.reverse();
}
```
