# Reto día #9

## 🎄Agrupando cosas automáticamente

### 🟥 Difícil

### Tenemos un montón de cajas en la fábrica de regalos... y como no automaticemos de alguna forma ordenar este desastre... ¡Igual nos quedamos sin Navidad!

```js
export default function groupBy(collection, it) {
  // ¡No olvides compartir tu solución en redes!
  const obj = {};
  const fn = typeof it === "function" ? it : (item) => item[it];
  const items = collection.map(fn);
  items.forEach((item, index) => {
    if (!obj[item]) obj[item] = [];
    obj[item].push(collection[index]);
  });
  return obj;
}
```

- [Link al reto 9](https://adventjs.dev/challenges/09)
- [Link al reto anterior](./reto8.md)
