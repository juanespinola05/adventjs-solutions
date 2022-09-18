# Reto día #4

## 🎄¡Es hora de poner la navidad en casa!

### 🟨 Normal

### Creo que ya podemos sacar el gorro navideño, el turrón... ¡Y el árbol de navidad! 🎄 Vamos a montarlo con JavaScript.

```js
export default function createXmasTree(height) {
  // ¡Y no olvides también poner los turrones!
  let tree = "";
  let chars = height * 2 - 1;
  for (let i = 1; i <= chars; i = i + 2) {
    let sides = (chars - i) / 2;
    tree += "_".repeat(sides) + "*".repeat(i) + "_".repeat(sides) + "\n";
  }
  let sides = (chars - 1) / 2;
  tree += "_".repeat(sides) + "#" + "_".repeat(sides) + "\n";
  tree += "_".repeat(sides) + "#" + "_".repeat(sides);
  return tree;
}
```

- [Link al reto 4](https://adventjs.dev/challenges/04)
- [Link al reto anterior](./reto3.md)
- [Link al siguiente reto](./reto5.md)
