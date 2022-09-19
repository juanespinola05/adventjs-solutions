# Reto día #11

## 🎄¿Vale la pena la tarjeta fidelidad del cine?

### 🟨 Normal

### ¡Este mes hay un montón de peliculones en el cine! Viendo que voy a tener que pasar bastante por taquilla también en 2022, estoy mirando de optimizar mis gastos. ¡Ayúdame!

#### Senior solution 😂 (jk)

```js
export default function shouldBuyFidelity(times) {
  // ¡No olvides compartir tu solución en redes!
  const TICKET_PRICE = 12;
  const normalTotal = times * TICKET_PRICE;
  const fidelityInitial = 250;
  const fidelityTotal = Array.from({ length: times }).reduce(
    (acc, _, index) => {
      let suma = acc + TICKET_PRICE * 0.75 ** (index + 1);
      return suma;
    },
    fidelityInitial
  );

  return fidelityTotal < normalTotal;
}
```

#### Normal people solution

```js
export default function shouldBuyFidelity(times) {
  // ¡No olvides compartir tu solución en redes!
  const TICKET_PRICE = 12;
  const normalTotal = times * TICKET_PRICE;
  let fidelityTotal = 250;
  for (let i = 1; i <= times; i++) {
    fidelityTotal += TICKET_PRICE * 0.75 ** i;
  }

  return fidelityTotal < normalTotal;
}
```

- [Link al reto 11](https://adventjs.dev/challenges/11)
- [Link al reto anterior](./reto10.md)
