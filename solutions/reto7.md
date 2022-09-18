# Reto día #7

## 🎄Buscando en el almacén...

### 🟨 Normal

### Tenemos un amigo que trabaja en una tienda y no es capaz de encontrar en el almacén los productos que tiene... ¿Le ayudamos?

```js
export default function contains(store, product) {
  // ¡Y no olvides compartir tu solución en redes!
  if (store === product) return true;
  if (typeof store === "object") {
    for (const key in store) {
      if (contains(store[key], product)) return true;
    }
  }
  return false;
}
```

- [Link al reto 7](https://adventjs.dev/challenges/07)
- [Link al reto anterior](./reto6.md)
- [Link al siguiente reto](./reto8.md)
