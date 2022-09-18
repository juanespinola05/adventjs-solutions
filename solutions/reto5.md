# Reto día #5

## 🎄Contando los días para los regalos

### 🟩 Fácil

### Estoy tan nervioso que no paro de contar los días que faltan 🤣. ¿Me ayudas creando un programita? ¡Venga!

```js
export default function daysToXmas(date) {
  // ¡Y no olvides compartir tu solución en redes!
  let xmasday = new Date("Dec 25, 2021");
  let daysLeft = (xmasday - date) / 86400000; // 1000 / 60 / 60 / 24
  return Math.ceil(daysLeft);
}
```

- [Link al reto 5](https://adventjs.dev/challenges/05)
- [Link al reto anterior](https://adventjs.dev/challenges/04)
- [Link al siguiente reto](https://adventjs.dev/challenges/06)
