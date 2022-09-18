# Reto día #2

## 🎄¡Ayuda al elfo a listar los regalos!

### 🟩 Fácil

### ¡Menudo lío 😵! Un elfo está ayudando a Santa Claus. Pensaba que le vendría ya ordenado de cada regalo cuantas unidades debe conseguir... ¡y le ha llegado una carta ✉️! ¡Ayúdale!

```js
export default function listGifts(letter) {
  // ¡Tú puedes!
  const letterArray = letter.trim().split(/\s{1,}/m);
  const regalos = letterArray.reduce((acc, curr) => {
    if (curr.startsWith("_")) return acc;
    acc[curr] = acc[curr] === undefined ? 1 : acc[curr] + 1;
    return acc;
  }, {});
  return regalos;
}
```

- [Link al reto 2](https://adventjs.dev/challenges/02)
- [Link al reto anterior](./reto1.md)
- [Link al siguiente reto](./reto3.md)
