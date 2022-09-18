# Reto día #1

## 🎄Contando ovejas para dormir

### 🟩 Fácil

### Con la emoción de que llegala navidad, nos está costando dormir bastante últimamente. Vamos a intentar usar este pequeño truco que nos ayudará a dormir más rápido 🐑.

```js
export default function contarOvejas(ovejas) {
  // aquí tu magia
  const ovejasFiltradas = ovejas.filter((o) => {
    let name = o.name.toLowerCase();
    return o.color === "rojo" && name.includes("n") && name.includes("a");
  });
  return ovejasFiltradas;
}
```

- [Link al reto 1](https://adventjs.dev/challenges/01)
- [Link al siguiente reto](./reto1.md)
